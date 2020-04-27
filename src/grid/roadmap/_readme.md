# Roadmap TF Grid

- [TF Grid 1.0.0](#tf_grid_100)
- [TF Grid 1.0.1](#tf_grid_101)
- [TF Grid 1.1.0](#tf_grid_110)
- [TF grid 1.2.0](#tf_grid_120)
- [TF grid 2.0.0](#tf_grid_200)

<a id='introduction'></a>
## Introduction

When we started this journey we originally intended to focus on the system administrator and application developer and provide an alternative to Amazon/GoogleCloud/DigitalOcean. We focused on computing & storage capacity (S3, Containers).

More and more it became important to deliver a True Decentralized alternative internet. A growing crowd of internet users wants to see a change, they want to own their data and be able to be on the internet without becoming a product. Our original vision did not cater enough for this requirement. Summer 2018 we decided to start developing a set of end-user application services that can run on top of the TF Grid. We are on track to launch in beta the first set of these services +-1 year after going in that direction. Starting 2020 we will launch our first set of end-user apps starting to provide options for real freedom to everyone on the internet.

This was a huge undertaking and most of this happened in the background without much publicity.
The services that will come out in Q1 will be a real revolution for the internet, as for the first time, it will be possible for everyone to be online and use an exciting set of products while maintaining full freedom, neutrality, and privacy.

As part of this decentralization requirement, we want any blockchain to be able to run on top of our TFGrid. Our TFGrid has a unique capability which we call **"Autonomous IT"** Think about it like self a driving car but then for Information Technology (IT). This makes it possible for any blockchain to run with more security and scale.

In Q1 2020 we will be able to demonstrate the "Autonomous IT" for the first time.

Below you can find our roadmap towards that goal.

<a id='tf_grid_100'></a>

## TF Grid 1.0.0 (active since start April 2019)
The Grid is only usable by application developers

### Services
- S3 storage service
- Virtual Zero-OS = container host (compatible with Docker)
- ZDB backend storage service
- Web gateway: how to make your service public

The above capabilities allow you to run most workloads which today would typically run on DigitalOcean or Amazon. Any app which runs on Linux can run on the TF Grid.
### Benefits
- No more docker images, flists allow faster deployment, 10x less storage and bandwidth required
- More security, because only signed files can run in the container
- More efficient storage enables lower costs (10x less power used)
- Can build any service on top

### Notes and Known Issues

- Not user-friendly, only meant for developers
- No user interface, only python scripting
- This is a pre-release version and the nodes are rebooted regularly and its data is erased (DO NOT RUN PRODUCTION !)
- Uses TFT from testnet (so free money)

<a id='tf_grid_101'></a>
## TF Grid 1.0.1 (June 2019)

Still non-production workloads and TFT's from testnet.

### Maintenance Release
- New JSX (jumpscale kosmos shell) release: easier to install/use
- Better documentation

### Example Workloads
Easy to deploy example workloads like
- Ethereum node example
- An Icecast node example
- A Minecraft server
- A Pastebin installation
- A PeerTube installation
- A multiplayer quake server (depends on licensing see http://ezquake.github.io/downloads.html)
- Odoo (ERP & Web Publishing system)
- Filemanager: see https://github.com/threefoldtech/tutorials/blob/master/tutorials/filestash/Filestash.py

<a id='tf_grid_110'></a>
## TFGrid 1.1.0 (June/July 2019)

- Ability to inform a 3bot about the life state of primitive which came life
- 3bot bootstrap
- Security on the deployment of vzos
- New web gateway
- Upgrade by rebooting of ZOS
  - the ZDB/s & virtual ZOS'es come life automatically

<a id='tf_grid_120'></a>
## TFGrid 1.2.0 (July 2019)

- TFChain no longer used for information storage
    - use BCDB

<a id='tf_grid_200'></a>
## TFGrid 2.0.0 (Q1 2020)

A Beta release which is using our self-driving IT capabilities.  The versions before this release have been available for testnet purposes.  While open and up and running for test workloads we learned a lot.  From this learning we concluded that some parts of zero-OS and some parts of the autonomous system where not good enough yet and therefore a major overhaul was done to some core components.  This also resulted in testnet no longer being available for developers.  Testnet will relaunch December 2019.

### NEW: Decentralized Apps

See 3BOT app doc

Our community asked us to focus on end-user facing apps for the first production release.
The names are not final, it could be they will change for launch.

- FreeFlow Pages (alternative to Facebook): everyone can now create their own '''Facebook'''
- FreeFlow Browser (browser running on the grid): privacy & freedom for all
- FreeFlow Connect (alternative to zoom/skype/hangout but decentralized): allow anyone to communicate, everywhere
- FreeFlow Files (filemanager, an alternative to e.g. dropbox)
- FreeFlow Blog / News / Wiki

for business users

- FreeFlow Biz (ERP system with CRM, …) based on Odoo
- FreeFlow Publish (wiki & web publishing system)

Everyone will be able to provide their private version of above-described apps on top of the grid.
All integrated with our 3bot mobile app.

### NEW: Blockchain As A Service

Help resolve the blockchain dilemma problem.

- Run HyperLedger (Ethereum compatible), Rivine (our own) on top of our TFGrid (more blockchains to follow)
- Human empowered blockchain: together with friends launch a blockchain, no-one can access or manipulate the blockchain, consensus required between the group to start or invalidate the blockchain.
- Benefits: easy = deploy a blockchain<5 min, cost-effective, much more secure (no-one can interact with the code), real decentralized

### NEW: BCDB = BlockChain DataBase

A True scalable blockchain Database.

- A true distributed, decentralized database (ledger)
- Store any information (e.g. contracts, …)
- It has all the features from a blockchain but not the downsides.
- Much more green & storage efficient (50x benefit compared to classic blockchain techno)
- Strongly Types schema support (complex types)
- Index & Search capabilities.
- Compatible with any chosen development language (Redis compatible API)
- Rich python client (userfriendly).

### NEW: 3bot = Your Digital Self

- Host your 3bot on the TF-Grid
- Multi-currency wallet (Gold, TFT, …)
- Your own data/identity (API driven)
- Integrates with 3bot mobile app

### NEW: “autonomous IT” preview (no production)

- Runs IT workloads with no people involved during operation, and has properties of a blockchain: consensus required for install, upgrade, remove.
- Ultra secure, gives hackers no chance because people are not involved in deploying or keeping the service up & running. There is nothing to hack.
- This is a preview release, only usable for real experts.

### upgrade to our compute & storage workloads

- Even more decentralized S3 server, where each users 3bot manages the S3 server
- Generic usable container service (docker conversion to container is supported)
- Web forwarding gateway (publish your services on the internet)

This service allows the running of any application you want on the decentralized grid.
As long as an application runs on the Linux operating system it can run on our grid.

### More decentralized apps

- FreeFlow Docs (office alternative running in the cloud) based on OnlyOffice
- FreeFlow Git (Alternative to Github)
