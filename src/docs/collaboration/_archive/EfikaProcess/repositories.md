# Efika Extranet Repositories

![](https://images.unsplash.com/photo-1453671424686-dfef17039343?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=9618389aa27a3979aced2cb4c9f68a4b&auto=format&fit=crop&w=1276&q=80)

A repository is location on an Efika Extranet where people work together around a specific topic.

Examples: 

- group of people working together in a scrum team
- a project repo where all content to do with a project is being stored
- a product repo where product people discuss everything to do with a product

these repo's have the following functions

- extranet for markdown documents (think about them like mini websites)
- issue management: keep track of bugs, tasks, ...

There are 2 types of repositories.

- content repo's
- scrum repo's

Think about them like a matrix

- horizontal = content (product, project, data, website, info, ...)
  - only issues used here = bugs, feature requests, tickets, questions
  - its where information lives
- vertical = group of people, working together based on stories & tasks = scrum
  - only issues used here = stories & tasks
  - its where process management is done (priorities, collaboration, ...)

## Scrum Repo's

- This is where peole work together
- Only used for **Organization** repositories \(org\_...\)
- Only place where we work with Story & Task issues.

### Organization repositories = SCRUM TEAM

* Always named as `org_$name`

* These are repo's which are specific to a group of people = [SCRUM TEAMS](scrum_team.md)
  
* Suggested standard organization repos:
  * org\$well chosen name for the group of people
  * e.g. org_development_cairo1

* Milestones
  * Defines a deadline \(date\) for the projects, there can be multiple, but tasks or stories can only belong to one
  * Freely chosen per project but they relate to a date, make sure they are consistent over repo's (easier for kanban)

* Types of issues in organization repos:
  * Story and Task

* Examples:
  * https://docs.grid.tf/threefold/org_marketing (which is a big team we use at threefold as example)

* Owned by the scrum team lead (which is not the manager, but the person who is at service for the full team).

* Information stored here is to let a team work together. It should not be content about a project, product, ... Its should be info required to let the team work, planning, scheduling, events, procedures only when specific to this team (otherwise refer to info_... repo) ...

## Content Repo's

Only place where we work with Tickets, Bugs, Feature Requests, Leads.

Do not put Stories or Tasks here.

Possible types of issues in Content Repo's:

  * Bug
  * Feature Request
  * Ticket
  * Question
  * Alert (result of some monitoring issue)

DO NOT PUT STORIES & TASKS in a content repo, they are meant to let people work together.

Types:

* **Home** repository \(home\)
* **Info** (content) repositories, single source of truth \(info\__..._\)
* **Data** repositories, have structure data \(info\__..._\)
* **Project** repositories \(proj\__...\)_
* **Product** repositories \(prod\__...\)_
* **ITEnv** repositories \(itenv\__..._\)
* **Websites** \(www\) repositories \(optional\) \(www\_...\)

### Home repository

* Only one per Efika Organization
* Always named `home`
* Starting point for people to find their way in all other repos in the Efika Organization

* Example:
  * [https://docs.grid.tf/threefold/home](https://docs.grid.tf/threefold/home)

### Project repositories

* Always named as `proj_$customer` or `proj_$customer_$projname`
  * Projects relate to customers or specific projects \(so not linked to a team\)
  * We use this to organize our work related
    * to 1 customer, only useful if customer project is large enough
    * to specific projects inside an organization if they are not linked to 1 group of people
  * Do not create specific `proj_$customer_$projname` unless if subproject is large enough

* Milestones
  * defines a deadline for the project, there can be multiple but tasks or stories can only belong to one
  * freely chosen per project but they are always linked to a date ideal to use same data as sprint.

* Owned by project owner \(sometimes called project manager\)


### Info repository

e.g. https://docs.grid.tf/threefold/info

single source of truth for information towards an Efika Organization.
There can be more than one but in TF we only went with 1.

### Product repositories

* Always named as prod`_$name`
* REMARK: is not part of Code Organization repo's, this is the commercial side of the business, belongs to a product manager

* Is product management / integration information.
 
* e.g.
  * how does the product relate to the component repo's \(underneath the Code Organization repo's\)
  * naming conventions
  * roadmaps \(customer facing\)

### ITEnv repositories

* Always named as `itenv_$environmentname` or `itenv_$customername_$environmentname`

* Is information about an it environment (there can be a zero-robot or JS9 config info inside)

* Milestones
  * Dates which means something for the env, e.g. getting in production date, or an upgrade date.
  * Ideal to use same data as sprint

### www = websites repositories

* Always named as `www_$name`
* Contains the code for a website
* Is simular to a code repo but this case for a website.
* When code changes website is updated and hosted automatically
* We use tools like caddy/hugo to automatically publish a website

* Milestones
  * Dates which means something for the env, e.g. getting in production date, or an upgrade date.
  * Ideal to use same data as sprint

### Data repo's

- they hold data in e.g. toml or json format
- example: https://docs.grid.tf/threefold/data_team  (normally private)