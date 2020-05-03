|  **Cloud Unit Definition v4** |  |  |  |  |  |  |  |  |
| --- | ---: | ---: | ---: | ---: | ---: | ---: | --- | --- |
|   |  |  |  |  |  |  |  |  |
|  **CU (Compute Unit) = MRU/CRU per month** |  |  |  |  |  |  |  |  |
|  GB Memory |  |  | 4 | 8 | 2 |  |  | = MRU |
|  nr vCPU |  |  | 2 | 1 | 4 |  |  | = CRU |
|  Passmark Minimum |  |  | 500 | 250 | 1000 |  |  | is performance cpu |
|   |  |  |  |  |  |  |  |  |
|   |  |  |  |  |  |  |  |  |
|  **SU (Storage Unit) = HRU/SRU per month** |  | HD (HRU) | SSD (SRU) |  |  |  |  |  |
|  GB Storage Capacity |  | 1,000 | 100 |  |  |  |  |  |
|   |  |  |  |  |  |  |  |  |
|  **NU (Network Unit = per GB) = NRU per month** |  |  | GB (NRU) |  |  |  |  |  |
|  GB transfered OUT or IN |  |  | 1 |  |  |  |  |  |
|   |  |  |  |  |  |  |  |  |
|   |  |  |  |  |  |  |  |  |
|   |  |  |  |  |  |  |  |  |
|  **Resource Units** |  |  |  |  |  |  |  |  |
|   |  |  |  |  |  |  |  |  |
|  cru = 1 logical core of CPU |  |  |  |  |  |  |  |  |
|  mru = 1 GB of memory |  |  |  |  |  |  |  |  |
|  hru = 1 GB of storage capacity on a harddisk |  |  |  |  |  |  |  |  |
|  sru = 1 GB of storage capacity on a SSD |  |  |  |  |  |  |  |  |
|   |  |  |  |  |  |  |  |  |
|  su = (hru / 1000 + sru / 100) / 1.2 | 1 SU is 1 TB of HD capacity, or 100 GB of SSD capacity |  |  |  |  |  |  |  |
|  cu = min((mru - 1) / 4, cru * 2) | max oversubscription on cpu core is 4 and min required mem is 4GB |  |  |  |  |  |  |  |