# JumpscaleX Installation Instructions

- [Prepare your machine](#prepare-your-machine)
- [Installation](#installation)

## Prepare your machine

JumpscaleX is currently supported for ubuntu and macOS, we will go through the installation process to be on a sanboxed container in your system.

### Supported Operating Systems

- Ubuntu 18.04 or newer
- macOS 10.7 or newer

Also we will need some requirments to be begin with. to install use the next command.

**Note** These packages are for ubuntu, for macOS users should have them already so skip this step

### Required Packages

- Open your terminal, or `press ctrl + alt + t` and type the following
  
    ```bash
    sudo -i; # this may ask you for your password
    apt update -y;
    apt install -y openssh-server locales curl git rsync unzip lsb python3 python3-pip;
    pip3 install click requests;
    ```

- Then this step is for both ubuntu and macOS

    ```bash
    pip3 install click requests
    ```

- Then we will make the following configuration which will give you an sshkey if you don't have one
  
    ```bash
    eval `ssh-agent -s`
    ssh-keygen
    ssh-add
    ```

- All configurations are ready. Next step is installation.

### Installation

- In your terminal execute the following, this will download the installer file, change its permission to make it executable

    ```bash
    curl https://raw.githubusercontent.com/threefoldtech/jumpscaleX_core/development/install/jsx.py?$RANDOM > /tmp/jsx;
    chmod +x /tmp/jsx;
    ```

- Then we can install our threebot using

    ```bash
    /tmp/jsx threebot;
    ```

