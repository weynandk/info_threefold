# This document shows how to setup/migrate your ThreeFold Farm and 3Nodes to TF Grid 2.0 (JSX Version)
NOTE: This guide is for experts. If you need assistance contact ThreeFold support via the chat on www.threefold.io

### Please make sure you read the  [V2 Networking Document](https://github.com/threefoldtech/zos/blob/master/docs/network/introduction.md) before you start migrating your farm/nodes. 

## Prerequisite: Install jumpscale container

See https://github.com/threefoldtech/jumpscaleX_core/blob/development/docs/Installation/README.md to know how to install jumpscale container

## 1. Register your identity on the TF Grid

As indicated in the install description start the kosmos shell inside your jsx container.  
Then follow these instructions to get register an identity and attach your farm to it.

Connect to the right network.
```python
j.clients.threebot.explorer_addr_set('explorer.grid.tf')
# j.clients.threebot.explorer_addr_set('explorer.testnet.grid.tf')  If you want to use testnet
```

Register your identity. To do so use `j.tools.threebot.init_my_threebot` function.
It takes 3 arguments

- name: This is your name on the grid. It must ends with .3bot'
- email: Email address link to this identity. Make sure to use a valid email address
- description: optional field. You can specify anything.

```python
j.tools.threebot.init_my_threebot(
    name='myname.3bot',
    email='myname@gmail.com',
    description="anything can go here")
```

## 2. Create a TF Farm

Now that your identity is known on the grid, you can create a farm.
To do so, you need to connect to the grid explorer 3bot.

```python
# get a client to the explorer
explorer = j.clients.explorer.default
# create a new farm object
farm = explorer.farms.new()
# name your farm
farm.name = 'my_super_farm'
# link the farm with your identity
farm.threebot_id = j.tools.threebot.me.default.tid
# Instruction below is only for farms which already exist in version 1.x and need to be migrated to version 2.0 !
# Specify the ItsYouOnline organization link to the farm
farm.iyo_organization = 'my_super_farm_v1'
# the tfchain wallet where the farming token neeeds to be paid. If this field is empty you won't be able to
# receive the farming token
farm.wallet_addresses = ['.....']
# email address where farming result and any information for farmer will be sent.
farm.email = 'myname@gmail.com'
# actually register the farm on the grid
farm_id = explorer.farms.register(farm)
# print your farmer ID
print(farm_id)
```

If the last function succeeded, your farm is now created.
If you go to the explorer web UI you should be able to see your farm in "All farms" dropdown list.

## 3. Create a bootable image

Use this bootstrap service: https://bootstrap.grid.tf, with farmer ID = the farm_id generated in step 2.  

## 4. Start 3Node with bootable image

After booting your 3Node it is visible on: [the tfgrid explorer](https://explorer.grid.tf)
