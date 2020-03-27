# tools for TEAL organizations

## intro

Teal organizations see: [Teal Organization](Teal Organization.md) is an amazing way to create new type of organizations.

There are special tools & special methodologies developed which can be used to try to manage such an organization see [holacracy](https://www.holacracy.org) and [glassfrog](https://glassfrog.com/).

We didn't research enough to already jump and go 100% for one of those yet.

There are not many organizations yet which have embraced this methodology and much is unknown.

There is an obvious example though which is how millions of people together develop opensource software using tools like github. These people voluntary work together organize themselves around accounts & code repositories. Tools like github are amazing powerful in letting these millions of people discover interesting projects on which they can contribute if they want.
People are proud on their projects, they want to have high quality, they are normally happy when other people find & contribute to their projects.

Lots of these projects are very high quality despite the fact that there is no central organization controlling anything.

I believe the lowest risk for us to experiment with this new organization way is to embrace this way of thinking and even re-use these tools.

The tools are rather complex and require training to be able to use them well but once you understand them the power is amazing.

The tools we describe in this document are only the beginning, we want to contribute to these tools and create add-ons which will make it easier for people to use these tools and have to learn less.

Unfortunately the first will have to learn a lot (-:



### only 6 tools to organize us

- github / gitlab (private):
	- what has been proven to work for millions of people generating opensource code in true collaboration without being in the same location also works for many more company workflows.
	- this tool can be used for 90% of our content generation as well as project management
	- it will required people to be flexible & adopt to new ways of working but its worth it
	- it has a learning curve though
- google docs/drive (or alternative, we are working with a partner on a private alternative):
	- mainly for the more designed docs like e.g. presentations (not for docs!)
	- excel is still the swiss army knife of choice for many tasks
	- do not use docs for proposals, white papers, ... all of this can be done in github/lab
	- the collaboration capabilities of gdocs are awesome but don't offer the traceability & fine level of control of github/lab.
	- we have a tool which exports content from google doc also in github/lab so we see what has been changed by who even if they used gdocs.
- telegram
	- ad hoc communication flows, use this to point people to the right info at the right time
	- this is the replacement for email
- content publishing system (doc generator)
	- which uses the info from multiple sources & creates a more userfriendly portal out of it.
- our secure edge cloud platform for processing & storage capacity
	- robots automate our life & secure our data
- our blockchain & identity management
	- for security & auditability (traceability)

I really believe that these tools are the ONLY tools required to run a company following all opinions expressed in this document. We are not there today but we can grow into this.

Only these tools will allow us to continuously publish all our information & outcome of our process in 100% transparency.

There is no need for separate
- CRM
- ticketing system
- issue management system
- task management systems
- budget reporting systems
- SLA management systems
- ...


## tools 

### markdown

A flexible text only format which can be used for

- contracts
- proposals
- websites
- specs
- white papers

In markdown the format is very limited & external formatters are used to convert to other formats like a website or pdf.

### git

@#TODO: *1 explain basics of git & why git can be used to manage a lot

is the basis of our tools.

- [git for the rest of us](http://www.infoworld.com/article/2886828/collaboration-software/github-for-the-rest-of-us.html)
- in case you want to become an expert and understand the underlying fundamentals read: 
	- [git guide](http://rogerdudler.github.io/git-guide/)


### toml / yaml

- two very easy formats to express structural information in 

toml example

```toml
[email]
from = "info@incubaid.com"
smtp_port = 443
smtp_server = ""

[me]
fullname = "Kristof De Spiegeleer"
loginname = "despiegk"

```

- this information can be also stored in git

### gogs / github

- are webbased tools with an easier interface on top of git.
- github we use for all our product components
- gogs we use for all other info e.g. company project management


### editing tools

We have re-packaged some open source tools to make it easy for working with the tools & formats as described above.

This package can be installed very easily and is supported by our engineers.

These tools are originally developed by developers for developers and as such they will have a learning curve to get started.

Once you reached a certain technical level you will be amazed to see how good your productivity will be. Anyone should be able to work with these tools in couple of days and while intimidating at first it will be much more easy afterwards and we are sure you will be thrilled by the advantages & productivity boost.

We will be constantly working on improving this toolset, it will become easier as we go.

The chosen components work cross platform and are free.

#### visual studio code editor 

- is a fantastic editor, originally created for developers but can be used by less technical people.
- has incredible support for markdown, toml, ...

#### troll commander (nice easy to use explorer of files)

- an easy to use flexible file manager, easier than command line to manipulate files.
- its a real productivity booster.

#### sourcetree

- graphical tool to manipulate git


#### google docs

- for spreadsheets & presentations we suggest to use google docs
- a private alternative to this is called only office (not to be used yet)
- we have developed tools which seamless integrate google docs with git so that changes & backups are accessible from git(gogs).
- please do not use google docs for textual documents, all of this can be done textual with markdown. 
- its a little bit getting used to but keeping e.g. contracts, proposals in git makes much more sense because of change management, version control, collaboration, ...
	- we have tools which can aggregate many sources of info to good looking proposals, ...

#### how to create diagrams (advanced users)

- preferably use tools like mermaid, dot, ... to in text form even create graphical elements, the output is not always very nice so its more suited for specs & internal docs.
- if diagrams need to be nice we recommend using google docs again 
- for design elements of e.g. websites, other tools can be used but this is rather the exception than the norm, its mainly important that all text stays in git (all info).

#### structural info

We believe its not needed to use specific database oriented apps like CRM, Accounting, ... but we realize this sounds not realistic. We are developing some tools which will demonstrate this approach. 

There are many advantages to this
- version control
- collaboration
- scalability
- security
- build in disaster recovery

all info as toml or yaml files in git.

#### how to store big files or directories

to be done


 


