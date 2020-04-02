# Deploying a flist

A flist is the container deployed on zero-OS. 
It can be converted from Docker or customized on the [Zero-OS Hub](https://hub.grid.tf/).
The result can be uploaded and made available in the flist repository, where it is available for usage.  

## Deployment of a flist through the chatflow

Within the 3bot Admin console, a chatflow has been created to deploy a generic flist. 

<img src=img/Chatflow_flist0.png width=200>

Through this chatflow, the kubernetes cluster is reserved and configured simply by collection of a number of parameters : 
- IPv4 vs. IPv6
- Number of worker nodes
- public ssh key (allowing to access the container using ssh)
- cluster secret
- network definition (choice between reuse of a netork that has been set up earlier or new one)
- ip addresses to access all workers

This information is sufficient to create the cluster.

<img src=img/kubernetes_chatflow11.png width=500>

If you choose to define a new network, this needs to be activated using Wireguard (see explanation on network).

<img src=img/kubernetes_chatflow12.png width=500>
<img src=img/kubernetes_chatflow13.png width=500>

Once this is done you can ssh into the virtual machine from your account that you used the ssh key from. 

<img src=img/kubernetes_chatflow14.png width=500>
<img src=img/kubernetes_chatflow15.png width=500>
