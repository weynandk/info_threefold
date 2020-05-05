

# How to set up your ThreeFold Farm

6 simple steps:

- [Create a identity using the 3bot login app](#create-a-identity-using-the-3bot-login-login-app)
- [Deploy a 3bot](#deploy-a-3bot)
- [Register your farm](#register-your-farm)
- [Download the EFI (UEFI) bootable image](#Download-the-0-OS-bootable-image)
- [Create boot medim](#create-boot-medium)
- [Boot your node](#boot-your-node)

## Create a identity using the 3bot login login app

Your ThreeFold Farm needs to be associated with an 3bot identity.

To create such an identity you need to install the 3bot app:

- [Android version](https://play.google.com/store/apps/details?id=org.jimber.threebotlogin&hl=en)
- [Iphone version](https://apps.apple.com/us/app/3bot-login/id1459845885)

## Deploy a 3bot

Check [this](threebot_server.md) document for details on how to deploy a 3bot.

## Register your farm

To register your farm, you first need to install the farm management app on your 3bot.
From the app store page on  your 3bot, install the "farm management app".

To install a new app on your 3bot: TODO

Once installed,click the big green cross on the top left corner:

![create farm button](new_farm.png)

Here you specify:

- **Farm name**: The name you want to give to your farm. This can be anything.
- **IYO organization**: if you owned a farm in the previous version of the tf grid. Specify the ItYouOnline organization attached to your farm. This is used to allow to keep the seniority of you farm.
- **TFT wallet address**: the TFT address where the the token earned by farming will be sent to each month
- **email address**: This email will be used if we need to contact you about your farm. The email will stay private.
- **Location**: optionally you can select the location of your farm on the map. If you don't, the location wil be deducted using geoip from your nodes.

![farm creation form](create_form.png)

Your farm is now created. You should see a new line in the "My farms" table.

Write down the ID of you farm in the left side of the table. You will need it for the next step.

![new farm](new_farm.png)

## Download the 0-OS bootable image

Go to https://dev.bootstrap.grid.tf to create your 0-OS image.

In the "Farmer ID" input field, enter the ID you received for your farm in the previous step. It needs to be an integer.

Then you can choose the different release of 0-OS. If you are not sure what to use, select "production".

TODO:...

## Create boot medium

TODO:

- create bootable USB
- use ipxe to boot form network...

## Boot your node

Boot your node with the USB drive and watch your farm management app in your 3bot. The node should appears there once they are booted.
