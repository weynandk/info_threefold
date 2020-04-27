
# Capacity to ThreeFold Token Index

To have a metric showing the underlying capacity supporting the TFT economy, we have developed a Capacity to Token index:

The capacity index value = commercial_value_of_grid (over 5 years) / nr_of_liquid_tokens (available today)

How do we measure the commercial index value?

- each node is being registered in the TF Directory
- the total resources available are measured by Zero-OS 
- the resources are measured through [resource_units](resource_units.md).

The following formulas are used to convert resource units to [cloud_units](threefold_cloud_units.md).

- 1 CU = min(MRU/4 x (1-5%),CRU x 2)
- 1 SU = HRU / 1093 + SRU / 92
- 1 NU = CU x 10 + SU x 2% x 1000

Each cloud unit has a commercial value at the time of writing (March 2019). We use

- USD 15$ for a compute unit
- USD 10$ for a storage unit

# Reasoning

We use as a basis the definitions in [cloud_units](threefold_cloud_units.md).

## Compute unit = CU

1 std CU is 4GB of mem and we take 5% buffer 
but we can never oversubscribe more than 4 times.
1 std CU has 2 virtual CPUs thanks to min CRUx2 we make sure that oversubscription is capped at 4.

We need to take minimum because the most conservative measurement needs to be used.

## Storage unit = SU

From experience, we know the required resources that allow us to deliver the specs as defined in the definitions.
It's the combination of SSD & HD capacity. 

The detailed calculations are described below.

## Hard disc capacity

= (archivecapacity x 70% + nascapacity x 30%) / redundancy_factor
= (1000 x 70% + 400 x 30%) / 0.75 = 1093

- 0.75 is the redundancy factor, which means we take 25% overhead for redundancy
- we take 70% of archive capacity in the field
- we take 30% of nas capacity in the field

## SSD capacity

= (SAN_disk x 40% x 2 + DB_disk x 10% x 2 + STD_disk x 50%) / redundancy_factor
= (30 x 40% x 2 + 5 x 10% x 2 + 60 x 50%) / 0.6
= 92

- For SSD we take 50% for std purposes, 10% is for database & 40% for SAN space
- The temp space is not redundant so there is no redundancy
- It's on SSD so the redundancy is 2x, we copy each block 2x
- 0.60 is the redundancy factor, which means we take 40% overhead for redundancy

## Network Unit

This is the most tricky one because we don't know the relation between network bandwidth requirements and storage or compute workloads. The NU's are a result of the available CUs and SUs.

We did the best estimates in this phase, this will improve as we get more data.

- compute_units x 20 + storage_units x 2% x 1000

## Estimation

- We estimate that averaged out each computing unit will require 20 GB of transferred data per month (which is conservative).
- We estimate that averaged out each storage unit will require 2% of its capacity transferred per month.


## Commercial Capacity Jan 2019

![](./img/token_value_calc.png)

- This is an example list of x farmers
- Each of them provide a certain amount of resource units
- We can calculate the provided cu/su/nu out of the resource units (formulas above)
- This results in the number of cloud units available
- We can then multiply the cloud units with commercial average prices on the grid
- This results in a total commercial value

The above example shows a USD 89,915,106 value  (Jan 2019)

## Token valuation Example

- if there would be a commercial value of 100m (+- summer 2019) and 500m tokens then the value would be $0.2
    - $100,000,000 / 500,000,000 = USD $0.2 per TFT
    
Disclaimer: This is only an example, starting september 2019 this will be calculated automatically.



