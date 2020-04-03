# Setting up a Network
## How to set up a network using the chatflows?

The network set-up is integrated in each of the chatflows (on ubuntu, flist, S3, kubernetes, ...). 

- If you haven't set up your network yet, select a new network : 

<img src=img/Chatflow_Ubuntu5.png width=500>
<img src=img/Chatflow_Ubuntu6.png width=500>

This network then needs to be defined using Wireguard. 
A different setup is needed on Ubuntu machines and on Macbook : 
- For Ubuntu machines, install wireguard using wg-quick
<img src=img/Chatflow_Ubuntu9.png width=500>
<img src=img/Chatflow_Ubuntu11.png width=500>

- On MacBook, please install the Wireguard application and define a new tunnel 
<img src=img/Chatflow_Ubuntu11.png width=500>
<img src=img/Chatflow_Ubuntu12.png width=300>
<img src=img/Chatflow_Ubuntu13.png width=500>
<img src=img/Chatflow_Ubuntu14.png width=500>

- If you previously defined a network, you can reuse an existing network.

<img src=img/kubernetes_chatflow6.png width=500>
<img src=img/kubernetes_chatflow7.png width=500>


## How to set up a network using the Jupyter Notebooks?
In the Navbar you will find the section "NEED THE NAME" that has pre-made notebooks. These will guide you through all the steps you need to take to setup a network, but do not limit you when it comes to parameter as you can edit the scripts as you go.

## How to set up a network using the CodeServer?
Within the SDK you'll find the CodeServer in the left hand navbar.
In here you will find all files and code you need to set up a network and have total control over it, set your parameters, choose your nodes, etc.
