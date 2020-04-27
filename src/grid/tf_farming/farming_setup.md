# Please note that the TF Grid is upgraded to version 2.0. This document will be updated pretty soon. If you want to add a farm and related nodes in the meantime please contact the [ThreeFold Support Center](https://support.grid.tf)

# How to set up your ThreeFold Farm

For the ThreeFold nodes to start recording farmed tokens, they need to run the Zero OS master branch.

6 simple steps:
- [Create an ItsYou.online organization](#iyo-org)
- [Register your farm](#register)
- [Download the EFI (UEFI) bootable image](#download)
- [Prepare your USB drive](#format)
- [Copy the downloaded EFI image to your USB drive](#copy)
- [Boot your node](#boot)

Also, see the [Threefold farmers' documentation](https://github.com/zero-os/home/blob/master/docs/farmers/README.md#configure-your-nodes).

<a id='iyo-org'></a>

## Create an ItsYou.online organization

Your ThreeFold Farm needs to be associated with an ItsYou.online organization.

To create such an ItsYou.online organization you need an ItsYou.online account. Creating one is simple, head to http://itsyou.online/ and follow the sign-up instructions.

Once logged in to your ItsYou.online account, also creating an ItsYou.online organization is simple.

Click **Organization** from the **Profile** menu in the top right corner:
![](https://raw.githubusercontent.com/zero-os/home/master/docs/farmers/images/iyo-organizations.png)

Now click **+ CREATE NEW**:
![](https://raw.githubusercontent.com/zero-os/home/master/docs/farmers/images/iyo-create-new-org.png)

And finally, specify the name of the new ItsYou.online organization and click **CREATE**:
![](https://raw.githubusercontent.com/zero-os/home/master/docs/farmers/images/iyo-create-new-org2.png)

> For the name of the ItsYou.online organization only lower case characters, numbers or spaces are allowed.

> The name of ItsYou.online organization needs to be globally unique, and therefor also referenced to as the **Global ID** of the ItsYou.online organization.


<a id='register'></a>

## Register your farm

Go to the ThreeFold Grid Capacity web site: https://capacity.threefoldtoken.com

![](./img/capacity.png)

In the top right corner click **Register Farm**:

![](./img/capacity2.png)

Here you specify:
- **Farm Name**: this can be anything, the name will be displayed next to your node in the listing of the capacity
- **Organization ID**: the global ID of the ItsYou.online organization you created in the previous step
- **TFT Wallet Address**: optionally you can also associate a ThreeFold Token wallet address to your farm
- **Farm Location**: location on the map of your farm

The result of your registration will be a JSON Web Token (JWT), which is your farmer ID (https://github.com/threefoldfoundation/info_foundation/blob/development/docs/definitions/farmer_id.md). Make sure to copy this token and keep it, because you will need it later in the process of setting up your nodes.


<a id='download'></a>

## Download the bootable image

On https://bootstrap.grid.tf click the **Assistant** button:

![](./img/assistant2.png)

In **step 1** of the Zero-OS **Boot Generator Assistant** page select Zero-OS branch `master`:

![](./img/branch_select_master.png)

Next, in **step 2**, specify the ID of the public ZeroTier network that connects all ThreeFold nodes in one shared network, the is ID `c7c8172af1f387a6`:

![](./img/zerotier_network_id.png)

In **step 3**, pass your ItsYou.online organization name (optional)and your `farmer ID` as a kernel parameter:

**NOTE: Please select 'Enable support flag' if you want ThreeFold to help you with any issue that might come up**

![](./img/howtosetupfarmstep3.png)

In **step 4** you find the download URLs for the bootable image in various formats, use the **EFI** format:

![](./img/choose_efi.png)

Or just copy the download URL into your browser:

https:// bootstrap. grid.tf /uefi/development/c7c8172af1f387a6/organization="yvesfarm" support farmer_id=your-farmer-id-here

![](./img/open_download.png)


<a id='format'></a>

## Prepare your USB drive

Start by connecting your USB drive to your computer.

In what follows screenshots from Mac OS X are used, but the principles are the same for Windows.

Search for **Disk Utility** in Launchpad and open it:

![](./img/disk_utility.png)

Select your USB drive and click **Erase**.

In the dialog that pops up  optionally enter a new name for the USB drive, and then select **MS-DOS(FAT)** from the Format dropdown menu:

![](./img/disk_utility2.png)

Click **Erase** which will format your USB disk and report about the result:

![](./img/disk_utility3.png)


The above can also be achieved from the command line:
```bash
diskutil list
diskutil eraseDisk FAT32 "ZOS" /dev/diskX
```

> Caution, in the above, replace `/dev/diskX` with the device file of your USB disk, which you can find by checking the `disk utility list` first, make sure to not shoot yourself in the feet here.

<a id='copy'></a>

## Copy the downloaded EFI image to your USB drive

Open **Finder** and select your formated USB drive from **Devices**:

![](./img/finder.png)

Create a root folder **EFI**:

![](./img/finder2.png)

![](./img/finder3.png)

In the new root folder create a subdirectory **BOOT**:

![](./img/finder4.png)

![](./img/finder5.png)

Locate your downloaded EFI image, here under the downloads:

![](./img/finder6.png)

Rename `ipxe-v1.4.1.efi` to `BOOTX64.EFI`:

![](./img/finder7.png)

![](./img/finder8.png)

Copy this file to the previously created folder `/EFI/BOOT` on your USB device:

![](./img/finder9.png)

![](./img/finder10.png)

![](./img/finder11.png)

And finally, eject your USB drive:

![](./img/finder12.png)

Or all the above from the command line:
```bash
mkdir -p /Volumes/ZOS/EFI/BOOT/
wget -O /Volumes/ZOS/EFI/BOOT/BOOTX64.EFI https://bootstrap.grid.tf/uefi/development/c7c8172af1f387a6/farmer_id=eyJhbGciOiJFUzM4NCIsInR5cCI6IkpXVCJ9.eyJhenAiOiJ0aHJlZWZvbGQuZmFybWVycyIsImV4cCI6MTUyODI4MzY3MSwiaXNzIjoiaXRzeW91b25saW5lIiwicmVmcmVzaF90b2tlbiI6IlBJcGQ4QmlfOXAyd1drYlB0dHQ4SEZpSEJXSk4iLCJzY29wZSI6WyJ1c2VyOm1lbWJlcm9mOnl2ZXNmYXJtIl0sInVzZXJuYW1lIjoieXZlcyJ9.8siq1Tk_b6ZzM675K4Aq3SYwS5J8Lk_5W5XSIbOrUgikJteTbmNzClOPNV1gTJVOFhfE4c-f1AEX2M4GM-Gs69cqpi1_YgXq_RPJvz6JuCbJdR8xBkJjgOfI7FS8PnUq%20development
diskutil umount /Volumes/ZOS
```

<a id='boot'></a>

## Boot your node

Boot your node with the USB drive and check the status of your farm on https://capacity.threefoldtoken.com:

![](./img/farm.png)

Under **Resource Units** you can click the **details** button which will bring up the details of the selected node:

![](./img/farm_details.png)
