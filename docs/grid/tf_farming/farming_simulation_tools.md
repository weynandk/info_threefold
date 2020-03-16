# Farming Simulation Tools


**Note: These tools help to estimate as good as possible the amount of TFTs, but are not producing binding results. Most AMD and INTEL CPUs are supported. INTEL NICs work in conjunction with Zero OS. Realtek NICs are mostly not supported. To find out if your hardware can be added to the TF Grid please [setup your farm and add the node to the TF Grid](tf_farming/farming_setup.md)**

<div style="overflow:hidden;">
   <iframe src="https://jscalc.io/calc/8jXXLOukrlXcI7H4" scrolling="yes" style="width: 100%; height: 582px; margin-left:0px;"></iframe>
</div>


**Inputs needed:**
- Number of logical cores: See your hardware specs (# of threads, example: 16 cores hyperthreaded = 32 logical cores)
- Amount of memory in GB: See your hardware specs
- Amount of solid-state disk (SSD) in GB: See your hardware specs
- Amount of disk storage (HDD) in GB: See your hardware specs
- Token price when capacity is listed in USD: Currently USD 0.12
- The set sales price for a compute unit [$]: USD 15.00 (until Grid usage start in Q1 2020)
- The set sales price for a storage unit [$]: USD 10.00 (until Grid usage start in Q1 2020)


*********************************************************************************************************

<div style="overflow:hidden; margin-top:15px;">
   <iframe src="https://jscalc.io/calc/3KL8gkvekUe52gGo" scrolling="yes" style="width: 100%; height: 774px; margin-left:0px;"></iframe>
</div>

**Inputs needed:**
- Number of computing units (CU): Output from Farming Token Estimator
- Number of storage units (SU): Output from Farming Token Estimator
- The sales price for a compute unit [$]: USD 15.00 (until Grid usage start in Q1 2020)
- The sales price for a storage unit [$]: USD 10.00 (until Grid usage start in Q1 2020)
- Average usage over 5 years [%]: we use 60% (realistic medium usage)
- Price erosion over 5 years [%]: we use 20% (lower than the industry as we are already multiple times lower in pricing).  The percentage set is applied over a period of 5 years where prices depreciate linear monthly the the selected percentage.  Total price impact of the period of 60 months is half the percentage.
- Average Token price (5 years) [$]: we use in our calculations USD 1.0

You can play around with the last three parameters to simulate different scenarios.

*********************************************************************************************************

<div style="overflow:hidden; margin-top:15px;">
   <iframe src="https://jscalc.io/calc/7PSBwT4Io6rQ9Bog" scrolling="yes" style="width: 100%; height: 582px; margin-left:0px;"></iframe>
</div>


**Inputs needed:**
- Number of tokens farmed [TFT]: Output from Farming Token Estimator
- Number of tokens cultivated [TFT]: Output from Cultivation Token Estimator
- Average Token exit value [TFT]: we use USD 1.0
- Hardware cost: See your hardware offer price or invoice
- Monthly operational cost: get an offer from a colocation partner (includes: rack space, power, connectivity)

You can play around with the average Token exit value to simulate different scenarios.

*********************************************************************************************************

Please contact the ThreeFold Support Center for any help:
- TF ticketing system: https://support.grid.tf/
- Email: support@threefold.tech

Sign up to the [Farmers' chat](https://t.me/joinchat/BwOvO0NpZjNMHFx8wD_5nw) to stay up to date on farming.
