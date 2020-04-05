## **How is data stored**

### ![huge archive](data_store1.png)

In most distributed systems, data is stored multiple times to guarantee redundancy.

This leads to a lot of overhead and is also not the most secure mechanism.

![400% overhead in regular systems](data_store2.png)

### **The "Space Algorithm" of storage**

![space algorithm image](data_store3.png)

Our system uses dispersed storage algorithms and is very different in nature.

![dispersed storage diagram](data_store4.png)

In a dispersed storage system the data gets dispersed in such a way that data will always be available even if 4 sites of the 20 (in this case) would not be available. Redundancy is the same as in the above example but the overhead is 20x less, it also has clear benefits from a security and efficiency perspective.

THis has been originally invented for communication in space.

### **How is this "Space Algorithm" used by the 3bot.**

![matrix image](data_store5.png)

By nature a 3bot is stateless (has no own data storage). A 3bot owns digital currency (TFT) which the 3bot can use to reserve raw storage and compute resources on the grid.

![3bot requests](data_store6.png)

Each 3bot has a unique capability to use this CPU and STORAGE capacity from the different TF nodes in the TF Grid in a safe and reliable way. Data cannot be lost because of above described dispersed storage algorithm.

A 3bot can store a petabyte of information as long as enough TFTs are available so the required resource can be reserved on the individual TF Nodes. 3bot is the only entity who has the required information and keys to make retrieval of the distributed data possible.

