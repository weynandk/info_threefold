# Farmer Program
![](img/farmingprogram.png)

ThreeFold created a simple Farmer Program for farmers to choose their type from.  Here are the main compoments in a high level overview:


|Farmer Type| Certified|Do It Yourself|
|-----------|----------|--------------|
|Server Hardware|Certified|any INTEL or AMD server not older than 4 years|
|SLA Contract with TF Tech|Yes|No|
TF Tech Support|Yes|No|
|Capacity Pricing|set by Farmer|set by Foundation (fixed)|
|Fee to TFT Tech|yes|no|





Farmers can opt in for Certification. Once certified the 3Nodes will mint more ThreeFold monthly than a DIY farmers 3Node. ThreeFold will with the help of the [ThreeFold Explorer](https://www.explorer.grid.tf) ckeck 3Nodes on quality achieved in relation to the certification contract. If the checks are not good enough the certification process will mark in the blockchain database (BCDB) which is used by the ThreeFold Explorer that the 3Node is no longer certified.

The following criteria are checked:

- Bandwidth: 24 times a day random non local nodes are used to upload a 2MB file to a 3Node. The bandwidth will be measured in mbit/sec

- Utilization: Through the ThreeFold Explorer the true utilization of the 3Node will be checked. It will be displayed in % of the 3Nodes total capacity.

- Uptime: The uptime per month will be created in the ThreeFold Explorer and is presented as percentage of 3Node availibility.


The foundation will give free certification to 3Nodes which benefit the distribution of capacity on the ThreeFold Grid. For example right now there is almost no capacity in Africa. Whoever puts boxes which are well distributed and sourced from a certified partner will not have to pay for the certification. The network uptime and capacity will still be measured and has to adhere to the certification criteria.


More details on how the Certification is implemented in the simulation can be found [here](https://github.com/threefoldfoundation/info_threefold/blob/development/src/grid/farming_logic_python.md)


Note: Until end of summer 2020 all farms and 3Nodes will be treated as certified. In the meantime farmers who are interested to become certified need to sign a contract with TF Tech in which the certification criteria are set. Once the contract is signed the farm will be measured against the certification criteria which shows exactly if the certification is deserved.