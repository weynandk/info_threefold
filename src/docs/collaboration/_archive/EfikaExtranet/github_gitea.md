## Why a tool like GitHub/GOGS/Gitea.

Git/GitHub is a most amazing tool to track changes and can be used in many more ways than people deem possible.

Millions of people use this in the world to collaborate. Mainly today for creating products, but it can be done for any other form of collaboration too.

We have selected the following tool combination for our Efika Agile Method

- Github: for all product related (code) repositories
- A modified form of Gitea for all other collaboration (we integrated with IYO = Itsyou.online)


We do realize that there is a learning curve to this method but we believe its the only way how hundreds of people who are everywhere can work together on projects.

### What can we keep in EE = Gitea

* coordination info e.g. procedures, ...
* any content (markdown) relevant for the repo (project or organization)
* Planning work \(stories in home repo, see [stories](stories.md)\)
* Specifications (specs) 
* Tickets from customers  (in project repo's)

Its important that all change is being tracked and people get visibility on everything which happened and is going to happen

### What can we keep in Github

all product related:

* Specs
* Documentation
* Planning work \(stories in home repo, see [stories](stories.md)\)
* Tracking of bugs
* Tracking of feature requests
* And of course all coding work using pull requests as a tool to track changes
* Its important that all change is being tracked and people get visibility on everything which happened and is going to happen


### Security & Clean Login Names

* If security is important to you make sure everyone uses 2-factor authentication
* If possible use clean login names on GitHub, many people use funny names which is nice but makes it hard for people to remember
  * Our suggested login names are  $first7lettersLastName+$firsLetterFirstname e.g. Kristof De Spiegeleer becomes _despiegk_


### Terminology Git related (advanced usage)

Git allows you to work with the content on your own computer and using an editor.
This is super powerful but a little bit more training is required.

When you want to use this more advanced/powerful way of working following terms will be handy.

#### Git

Git is an open source program for tracking changes in text files. It was written by the author of the Linux operating system, and is the core technology that GitHub, the social and user interface, is built on top of.

#### Markdown

Markdown is an incredibly simple semantic file format, not too dissimilar from .doc, .rtf and .txt. Markdown makes it easy for even those without a web-publishing background to write prose \(including with links, lists, bullets, etc.\) and have it displayed like a website. GitHub supports Markdown, and you can learn about the semantics here.

#### Branch

A branch is a parallel version of a repository. It is contained within the repository, but does not affect the primary or master branch allowing you to work freely without disrupting the "live" version. When you've made the changes you want to make, you can merge your branch back into the master branch to publish your changes.

#### Clone

A clone is a copy of a repository that lives on your computer instead of on a website's server somewhere, or the act of making that copy. With your clone you can edit the files in your preferred editor and use Git to keep track of your changes without having to be online. It is, however, connected to the remote version so that changes can be synced between the two. You can push your local changes to the remote to keep them synced when you're online.

#### Collaborator

A collaborator is a person with read and write access to a repository who has been invited to contribute by the repository owner.

#### Commit

A commit, or "revision", is an individual change to a file \(or set of files\). It's like when you save a file, except with Git, every time you save it creates a unique ID \(a.k.a. the "SHA" or "hash"\) that allows you to keep record of what changes were made when and by who. Commits usually contain a commit message which is a brief description of what changes were made.

#### Contributor

A contributor is someone who has contributed to a project by having a pull request merged but does not have collaborator access.

#### Diff

A diff is the difference in changes between two commits, or saved changes. The diff will visually describe what was added or removed from a file since its last commit.

#### Merge

Merging takes the changes from one branch, and applies them into another. This often happens as a Pull Request \(which can be thought of as a request to merge\), or via the command line. A merge can be done automatically via a Pull Request via the GitHub.com/Gitea web interface if there are no conflicting changes, or can always be done via the command line. See Merging a pull request.

#### Pull

Pull refers to when you are fetching in changes and merging them. For instance, if someone has edited the remote file you're both working on, you'll want to pull in those changes to your local copy so that it's up to date.

#### Pull Request

Pull requests are proposed changes to a repository submitted by a user and accepted or rejected by a repository's collaborators. Like issues, pull requests each have their own discussion forum. See Using Pull Requests.

#### Push

Pushing refers to sending your committed changes to a remote repository such as GitHub.com. For instance, if you change something locally, you'd want to then push those changes so that others may access them.

#### Remote

This is the version of something that is hosted on a server, most likely GitHub.com. It can be connected to local clones so that changes can be synced.

#### SSH Key (advanced)

SSH keys are a way to identify yourself to an online server, using an encrypted message. It's as if your computer has its own unique password to another service. GitHub/Gitea uses SSH keys to securely transfer information from GitHub.com to your computer.

#### Upstream

When talking about a branch or a fork, the primary branch on the original repository is often referred to as the "upstream", since that is the main place that other changes will come in from. The branch\/fork you are working on is then called the "downstream".

#### Blame

The "blame" feature in Git describes the last modification to each line of a file, which generally displays the revision, author and time. This is helpful, for example, in tracking down when a feature was added, or which commit led to a particular bug.

### magic comments

We support some 'magic' comment that you can use in issue and help to manage story and tasks.

`!! prio $prio` Set the prioriry of an issue. $prio is checked on first 4 letters, e.g. critical, or crit matches same

`!! p $prio` alias above

`!! move gig-projects/home` move issue to this project, try to keep milestones, labels. if it's a story, move all the tasks related.


REMARK: is not enabled yet but planned. 