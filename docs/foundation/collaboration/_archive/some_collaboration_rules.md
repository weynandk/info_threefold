# intro

@TODO *1 write intro why we do this

# rules

## single source of truth is in a git repo (e.g. gitea e.g. this repo)

All information (not representation) is stored in git repo's this gives us traceability and very good colaboration possibilities.

Avoid ad hoc word or google documents, put information in the right project repo (see below), sometimes it makes sense to collaborate in a google doc but keep markdown format & then every so often copy this content to git (which is still the master).


## use projects's = git-repo's to organize work

- each project is a repo in git
- different types
    - ```home``` : the home repo for an account e.g. for threefold, its the starting point, its like your home page for your conmpany or organization
    - ```org_...```: org = organization
        - is a group of people working around a certain vertical set of work e.g. support, operations, ...
        - they use this project to talk about how to improve their organization 
        - all info relevant specific to their organization is in this repo (make sure info is not duplicated from proj_...)
        - these projects are never ending
    - ```proj_...```: proj = project
        - projects with multiple milestones
        - can be related to a customer or can be internal
        - people from multiple organizations work on projects
        - examples could be a deployment if a IT solution with a customer, it could be a project to improve infrastructure, ...
    - ```prod_...``` : product
        - a product which is being developed, it links to the software repo's which are e.g. on github
    - ```itenv_...``` : IT environment
        - describes the deployment of an IT system with info (often private) how to manage, deploy, ...
        - sometimes this uses Jumpscale AtYourservice technology to deploy changes
    - ```info_...``` : information
        - when the repo is non of above and only used to store information (can be structural info) then info_... is used
    - ```www_...``` : website
        - autopublished by tools like hugo
- each project has a promotor & guardian: define this on home page
- make sure proper readme.md file (home page) exists
    - goal of repo
    - who is guardian,promotor
    - link to milestones
    - link to other info
    - link to other repo's which are relevant for this one
    - link to the telegram channel or group used for this repo
    - link to google drive folder
- use telegram to announce important changes or ask for colaboration
    - use as name $companyShortName_$reponame (lowercase) as the name of group or channel
    - put the link to this group/channel on readme.md
    - only use it to announce changes, ask colaboration, news to do with project
- use milestones to organize work
    - milestone is put on a repo in e.g. gogs/github
    - its a date with well specified deliverables
- issues are used to specify what needs to be done or is required
- issues types
    - type_feature
        - describe a feature you want for a product, organization, project
        - its the request for change basically
    - type_task
        - underlying tasks, they can execute work on a feature or story
    - type_question
        - anyone can ask a question
    - type_ticket
        - customer interaction, customer needs something, we need to follow up to make sure customer is happy
    - type_alert
        - a monitoring system or person has escalated an alert, its a state to show that something is not working & attention is required e.g. server is down
    - type_story
        - see scrum
    - type_bug
        - a defect in the project, needs to be resolved
    - type_knownissue
        - its a defect which will not be resolved but it describes for the user what e.g. a workaround is or when to expect a solution

## use & learn & stick to the tools

- see this list of [recommended tools](https://docs.greenitglobe.com/teal.university/whatis/src/master/tools_for_teal_organizations.md)
- we realize there is a learning curve to master these tools but longer term its for sure worth it

## google docs is not a bad choice for non textual information

e.g. pdf's, presentation & spreadsheets

- organize your work in google drive organize per company and re-use the reponames as specified above
    - $company_$reponame e.g. gig_org_support, share directly on this level
    - only share & do security at this level
- only store 
    - pdf's
        - e.g. customer sends you info
        - e.g. signed contracts
    - presentations
        - do not just copy, try to work with a master presentation & then create versions out of it for specific projects/customers but keep master up to date
    - spreadsheets
    - short living colaboration docs
        - e,g, some brainstorming document, or online changing meeting document
- DO NOT
    - store original other documents in gdoc e.g. powerpoint preso's, try to convert

## only keep active & used data in the repo's or google drive folders

- its important that only relevant information is kept visible in the repo's
- how to work with information not ready to be used yet
    - git
        - branch
        - or _beta folder
    - gdrive
        - _beta folder (which is subfolder of each relevant folder)
- what to do with info which is no longer relevant or you don't know its relevant
    - git
        - just delete, git keeps all history
        - or exceptional if you want the history to be more visible _archive folder
    - gdrive
        - _archive folder (which is subfolder of each relevant folder)
- do clean up regularly !!!
- the guardian is responsible for making sure that all contributors follow the rules & the repo/gdrive folder is clean & organized

## use links

- in google docs/preso/excel or markdown documents, use links to link to other relevant information
- make it easy for your users to find info !!!

## do not destroy work, improve it

- if people have created something be respectful for it, try to improve if not possible go back to them and see how to get from the current situation to the required one.
- the promotor & guardian of a repo is the final responsible people for the quality of their repo/gdrive folder

