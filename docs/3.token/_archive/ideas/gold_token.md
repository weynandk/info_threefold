## Ideas

- gold token per region e.g. Europe/Dubai
- gold supplied & kept by preferential partners
- we find at least 3 banks who will provide the online accounts for 

## digital currency flow

### gold direct

- customer has existing bank account
- customer does KYC with ItsYouOnline (if not done yet)
- customer has all info on ItsYouOnline (addr verified, tel, email)
- gold partner accepts KYC if not older than e.g. 12 months (tbd).
- gold partner allows customer to buy gold token X (done per partner)
- gold token stored on wallet of customer

### bank partner path

- customer gets ebank account with our new banking partners
- bank does KYC
- bank makes relations ship with our gold partners
- gold partner accepts KYC & other customer info from bank partner
- banking partner resells gold partner gold token X
- gold token stored on wallet of customer

# Technology

## Components (definitions)

### ThreeFold Wallet

- runs in virtual machine on user desktop or in TF Grid in Secure Execution Engine (see below).

### Digital Me (DM)

- first version of digital.me hosts personal information for a user
- info stored
	- contact info (email, tel, addr, ...)
	- news/info to others (per group or public)
	- calendar info (phase 2)
- each digital.me has a unique id and unc name e.g. kristof.de.spiegeleer (at least 3 parts)

### ItsYou.Online Service (IYO)

- = identity verification service / system
- the ThreeFold Foundation runs this service on the TF Grid.
- verifies email, sms & address.
- can execute & verify KYC
- important: does not store any information !!!
	- all info is in digital.me's
	- it just sign's the digital.me info like email addr, ...
- its basically a web & rest interface on top of data in digital.me
- oauth2 authentication engine, stateless and talks to digital.me backends.

### Secure Execution Engine (SEE)

- secure operating environment which hosts
	- digital.me code (digital identity of people)
	- ultra secure wallet for digital & fiat currencies
	- clients to blockchains
	- decentralized exchange
- each SEE runs on dedicated hardware (or virtual machine on TF grid)
	- only 1 user per SEE !!!!
- unique secure operating system = zero-os
- runs on small embedded computer (arm based)
	- hardware = computer 100% neutral, backdoor free
	- all firmware of cpu, network chips, bios = open source
	- all firmware audited for avoidance of backdoors
- operating system = 100% neutral, opensource, reliable
	- audited & built by 10 indpendent technical guardians (ThreeFold guardians) 
	- minimalistic = more security
		- no shell in core of OS (e.g. no SSH server)
		- no local state, all secure data only available in memory

### Secure Web Remote IO (SIO)

- the applications run securely inside the SEE
- some of the information is securely exposed over web API's 
- sensitive information can only be entered using the SIO.
- The SIO is a super secure mechanism where output of the application gets streamed over a secure channel into your browser, the output gets rendered in your browser, if the user types anything or uses mouse the commands are sent back over the secure channel to the app.
	- think about it like your browser becomes the screen/keyboard/mouse for the app which runs inside the SEE
	- no logic runs inside your browser, only visualization and input/output redirection happens there
- this is the most safe mechanism to allow anyone to interact with their wallet or digital me.

### Decentralized Exchange

Allow customers to exchange +- any digital currency to any other digital currency with NO EXCHANGE FEE and 100% secure.

No centralized parties are in the middle which can benefit from the information you have put.

Every wallet puts their orders on an orderbook (for now hosted by TF).
The wallets talk to each other directly and use atomic swaps to allow exchange between digital currencies with no exchange fee !!!


## how does it work

- each user has a digital.me account which is owned by the user.
	- ideal for Europe data protection law
	- this digital.me account has contact & kyc info (verified by IYO)
	- runs in Secure Execution Environment (SEE)
- a private wallet runs in same Secure Execution Environment (SEE)
- the banking partner has agreement with their investment partner (which is the gold partner).
- legally spoken the bank is not in crypto world.
	- The bank allows their customers to buy/sell/keep gold starting from their bank accounts.
	- The users own their own wallets (no centralized part)
	- The user exchanges between the Gold Token and any other Digital Currency with no exchange fee from their own privae wallet.
	- If the user wants to go back to fiat, the user goes to gold tokens first.
	- Then the user sells the gold tokens & gets fiat on their account
- If the bank wants they can allow the user to use the TF Wallet and connect to their ebank account in a seamless matter.

# Why is this so good & needed

Digital currencies are there to stay and they give a lot of security, freedom and convenience to users.

But today

- most digital currencies are 
	- not green (mining is super dirty for the plannet)
	- slow (1h for BTC)
	- not scalable
	- expensive (high transaction fees)
	- abused by centralized exchanges
	- speculative: not stable enough for real commerce
	- no real utility: how many digital currencies are used for real business?
	- no support for micropayments
	- many people are too afraid about using them because of image of these crypto currencies today, there is need for clean ones

There is need for

- reliable onboarding mechanism (through existing reputable banks)
- reliable, stable, backed tokens (e.g. ThreeFold Token, e.g. Gold Token)

Because of our unique technology and the ThreeFold grid we can execute on this vision and give people access to digital currencies with all safety and 100% in line with regulations.

# partners

## banking partner

### requirements

- proper bank with required bank licenses
- set of API's which allows the customer TF Wallet to 
	- seamlessly deal with money transfer to and from gold tokens
	- see fiat status on bank (currency, amount, transactions)
- ability to execute this < 3 months (end2end)

### why would banking partner wants this

- through the gold token & decentralized exchange bank gets into digital currency world without risk
	- only has to deal with gold token partners
	- these partners are known and processes understood
	- tokens are backed by real assets
	- all 100% confirmed to known regulation (token is just a mechanism to streamline who people can buy/sell gold, using a reliable blockchain)
- transaction fees
- image = modern
- bank customers get access to invest in large majority of all digital currencies without any risk & legal exposure

## gold partners

### requirements 

- audited procedures about where gold is kept
- validation (audited) there is enough gold to back the tokens
- reporting (audited) about the gold amount
- gold partner uses the token blockchain as backend for his operation

### why would gold partner want this?

- lots of additional volume (transaction fees)
- blockchain as more secure way to buy, track & audit the gold
- is a business model ready for the future

### we need info

- location
- who is behind 
- amount of gold traded (physical vs online) per day

## technology partner = bettertoken

- delivers/maintains the blockchain technology to the bank/gold partner
- features
    - scale
    - fast transaction times
    - reliable
    - safe
- cost
	- tbd:EUR 100k startup + ?% on chosen transaction fee by (but min EUR 5k/month)

# The link with ThreeFold Token (TFT)

## the most valuable, green and reliable token in the world

the 3 values of the token

- TFT is a super valuable token.
	- backed by fastest growing commodity in the world = the internet
- TFT is good for the planet
	- no dirty mining, TFT is result of green farming of internet capacity
- TFT is reliable
	- scalable & secure thanks to our own blockchain rivine
	- easy to exchange: supported in our own Decentralized Exchange using atomic swaps
	- fast: <10 sec for transaction, <2 min for full verification
	- hosted on the ThreeFold Grid which is reliable & neutral

## TFT will be a real utility

A lot of effort will be done in getting this token to be used for real life usecases. People buying & selling...

A first example is "

