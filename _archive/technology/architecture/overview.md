## Architecture Overview

### What problem is TF TEch solving?

ThreeFold tech has developed technology that aims to break through barriers.  Current barriers for prolifiration of technology throughout the world are financial and technology:
- **Finanicial**. Not all global citizens have access to a bank account and complementary credit/debit cards.  Therefore the current digtial service providers are not accessible for all.  In order to break through this barrier a digital currency is needed.
- **Operatinal**. The current internet and its digital services rely ion networks connecting central datacenters to decentralised users.   This works well for the people that live in close proximity of these datacenters but is increasingly comples (and more expensive) for people that live further away from these datacenters.  To create efficiencies the datacenter needs scale, the large facilties are the more efficient the datacenter model gets (number of devices managed per person increases).  The downside of larger scale is that these datacenter can only exists in locations where there is sufficient density of power (electricity), capcital, people and knowledge.  This makes datacenters only feaisble in the developped world and not very far outside of that.  In order to break out of this impasse, internet capacity and services have to be created by using less power, less capital, less people and lesss knowledge. 

![](images/datacenter_large.png)

So to break these two major obstacles ThreeFold tech has developed technology that allows anyone that owns (or purchases) hardware to create a grid out of this hardware that operates [autonomous](https://www.merriam-webster.com/dictionary/autonomous).  The technology allow for autonomous operations of capacity that performs compute and storage workloads and creates a thrue peer 2 peer grid of capacity for private or public use cases.

### What is a smart contract for IT?

!!!include:smart_contract_for_it.md

#### Smart contracting (1+2).

Every personand and/or legal entity is represented on the grid by a digital avatar called a "3bot".  This  3bot has capabilities to represent persons or legal entities in a unique way in the following areas:
- a unique digital identity
- a unique digital currency wallet
- capabilities to query, search, find and communicate to other 3bot's in a securely (encrypted) peer2peer (3bot to 3bot)
- extend capabilities by creating new knowledge (code) 

With these capabilities the digital representation of people and legal entities can do most negotiation for search, find and contracting for services or capacity without human intervention.  An example of that process is listed below. 
![](images/grid_provisioning2.png)

Based on search requirements specified by the user (preferred geo, price, availability, etc. etc.) the 3both will find producers of capacity which match the criteria of the user and conduct a negotiation process to meet the producers terms and conditions and meet all of the users requirements.  Once all agreed, a digital currency transaction is done and the IT expert / Farmer accept the capacity reservation.

Technology repositories:
- [Jumscale libraries](https://github.com/threefoldtech/jumpscaleX_core)
- [3bot](https://github.com/threefoldtech/jumpscaleX_threebot)

#### Contract storage: Blockchain database (3)

The blockchain database is the centre piece of the architecture.  A blockchain database is a [database](https://en.wikipedia.org/wiki/Database) that has all the properties of database extended with blockchain characteristics.  A database has (indexed) records of data that are easy to retrieve (performance) and can change, databased record are meant to be updated periodically.  The blockchain database work along the same principle but add blockchain characteristics to the record changes, records are immutable and every record that has to change results in a new record being created with a link (chain) back to the original record.

This blockchain database is use to store the result of the peer2peer nogotiation conducted and completed by the two 3bots.  It only contains the relevant data required to describe what as agree in the negotiation.  Things like unique identities of the parties involved, quantity and duration of the capacity rent and very importantly which systems are to be involved in delivering this.

As this blockchain database is always append and has immutable records by definition we now have a 100% accurate record of all agreements struck between providers and consumers in very little details required to actualy deploy workloads.  And this is where the magic starts happening because the consequence of having a 100% accurate record you can restart failed parts of IT architectures with having to intevene.

#### Hardware and capacity creation (5)

Capacity creation happen by independent people who own or invest in hardware (at this point in time it has to be an Intel or AMD CPU) hardware and install the ThreeFold operating system.  This operating system is designed to be a bare minimum operating system providing minimal is very secure and 