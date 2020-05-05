![](./img/diy_farming.png)

# Farming Program

ThreeFold created a simple Farming Program for farmers to choose their type from.  Here are the main compoments in a high level overview:


|Farmer Type| Certified|Do It Yourself|
|-----------|----------|--------------|
|Server Hardware|Certified|any INTEL or AMD server not older than 4 years|
|SLA Contract with TF Tech|Yes|No|
TF Tech Support|Yes|No|
|Capacity Pricing|set by Farmer|set by Foundation (fixed)|
|Fee to TFT Tech|yes|no|

Farmers can choose for certified hardware. Once certified, a 3Nodes will mint more [ThreeFold Tokens](token_what.md) monthly than a DIY farmers 3Node. ThreeFold will verify the quality achieved by 3Nodes on the [ThreeFold Explorer](www.explorer.grid.tf) to ensure they perform according to the certification contract. The moment a 3Node performs under the certification standards, the information will be added to the blockchain database (BCDB) used by the ThreeFold Explorer and the 3Node will loose its certification level.

The following criteria are verified:

- Bandwidth: 24 times a day random non local nodes are used to upload a 2MB file to a 3Node. The bandwidth will be measured in mbit/sec

- Utilization: Through the ThreeFold Explorer the true utilization of the 3Node will be checked. It will be displayed in % of the 3Nodes total capacity.

- Uptime: The uptime per month will be created in the ThreeFold Explorer and is presented as percentage of 3Node availibility.


The Foundation will give free certification to 3Nodes which benefit the distribution of capacity on the ThreeFold Grid. For example right now there is almost no capacity in Africa. Whoever puts boxes which are well distributed and sourced from a certified partner will not have to pay for the certification. The network uptime and capacity will still be measured and has to adhere to the certification criteria.


More details on how Certification is implemented in the simulation can be found [here](https://github.com/threefoldfoundation/info_threefold/blob/development/src/grid/farming_logic_python.md)


***Note: Until end of summer 2020 all farms and 3Nodes will be treated as certified. In the meantime farmers who are interested to become certified need to sign a contract with TF Tech in which the certification criteria are set. Once the contract is signed the farm will be measured against the certification criteria which shows exactly if the certification is deserved.***