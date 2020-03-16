## Stories are the Start of All

![](https://images.unsplash.com/photo-1456324504439-367cee3b3c32?ixlib=rb-0.3.5&s=45160e59ac36a57dce0ec249a7b75161&auto=format&fit=crop&w=1350&q=80)


Stories help us to organize our work. They need to comply to certain requirements to be effective though.

A story normally represents the view of a person, e.g. "I as product owner for product X would like to see Y features to be implemented because... customer Z needs this... our strategy is..."

Writing user stories may seem to be simple but there are many ways you can mess it up (Incomplete, inconsistent or missing valuable parts such ass acceptance criteria/DOD), to avoid this common mistakes, We have created this list of the most common pitfalls you must avoid while creating your stories.  [see the story pitfalls](story_pitfalls.md)

Stories are pieces of work (not simple tasks) which are aggreated in a story = its like a card you would stick on a whiteboard.

**Stories can exist in Trello Board or in scrum repo's : org_...** on our Efika Extrante (EE)

### Properties

- Well chosen name
- Clear description of what we want to achieve
- Some Minimal description of deliverables and requirements (don't write specs here, they are markdown docs see below)
- Story Card owner:
    - best to only have 1, is linked to the story
- Estimation of the effort in days or hours (optional)
    - this needs to be redone on max 2 daily basis by story card owner
    - best to put this in title e.g. [2d] or [8h]
- A story needs to have a beginning & an end
- A story should never take longer than 1 month, if it is longer create 2 stories.


**Use links to put structure in story**

- Links For Non Product Related Story (URLs) to
    - Specifications (link to wiki, source = markdown document)
    - Questions/Bugs/FR (links to issue on EE)
    - Tickets (links to issue on EE or to trello cards in other non story board)
- Links For Product Related Story (URLs)  to
    - Specifications (requirements, code examples, ...) (in code github repo as markdown document)
    - Features or bugs which are related to the story (in code github repo as markdown document)


### Usage In Trello

- optional: define a priority = a label
    - Critical (Red)
    - Urgent (Orange)
    - Normal (is no label)
    - Minor (Green)
- Milestone: 
    - the swimlane in the story board (is the vertical column) 
        - e.g. this_week, future this_month
- but the tasks inside a checklist in the story
- Format:
	- Title: ```Story title``` [```time left e.g.4d```] e.g. Onboard the first 100 guardians [10d]


#### Title: ```$storyDescription``` ```[$time]```

- The time estimate is in title, this is the remaining time for this story
    - this is only set by the story card owner !!!
    - this needs to be set on max 2 daily basis !!!
    - time is working time (sum over all people)
    - this is an estimate this is not the sum of the times used inside the story or specs underneith

#### Body


requirements & remarks are optional.


```
## GOAL:

Clearly describe what needs to be achieved.

## DESCRIPTION

Describe what story is about.

## REQUIREMENTS:

- very high level overview and/or links to requirements (which are in code repo)
    - only the high level overview, the rest is in the code repo's

## REMARKS:

- List all remarks
 
```

### Usage in EE = Efika Extranet

- Priority set as label (optional):
    - Critical (Red)
    - Urgent (Orange)
    - Normal (is no label)
    - Minor (Green)
- Milestone: 
    - a label, linking the story to a specific date e.g. march = is linking to the sprint
- Assignee: is the [story card owner](roles.md)
    - only 1
- Links to tasks which are stored in same repository
    - [see tasks](task.md)


#### Title: ```$storyDescription [4d] ($storyname)```

- Title: ```Story title``` [```time left e.g.4d```] (```Story name```)
- The story name is used as reference in [Tasks](task.md) related to the story
- See [specs](specs_format.md) for definition time estimates.
- The time estimate is in title, this is the remaining time for this story
    - this is only set by the story card owner !!!
    - this needs to be set on max 2 daily basis !!!
    - time is working time (sum over all people)
    - this is an estimate this is not the sum of the times used inside the story or specs underneith

##### Body

see [specs](specs_format.md) for definition of task tables and time estimates.

```
## GOAL:

Clearly describe what needs to be achieved.

## DESCRIPTION

Describe what story is about.

## TASKS (ONLY in case of EE, otherwise a checklist in Trello)

- [ ] [crash in server ... on env ...](https://something)
- [x] [fr, nicer UI for page ...](https://something)
- [ ] [don't forget to copy the code to ...](https://something)
- [x] ask feedback to kristof about specs on this task

- is an optional task table, [see tasks](task.md)
- use this table as a high level overview and as a way how to calculate how much needs to be done.
- Tasks are always stored in the same repo as where the stories are located !!!

## LINKS

...

## REQUIREMENTS:

- very high level overview and/or links to requirements (which are in code repo)
    - only the high level overview, the rest is in the code repo's

## REMARKS:

- List all remarks

```


### When does a story card go into VERIFICATION stage?

- For stories related to projects or customers:
	- When work or subproject is done and is ready for VERIFICATION

- For storries related to code:
	- When code/story completed
	- When autotests (if relevant) are created
        - When autotests are already executed and succesful.
	- When all documentation relevant to the story is done
		- Do not forget to document how to test the story card
		- Do not forget to document on how to install/build everything related with the story card
	- When all tests are done


### When is a story card complete (DONE)

- When VERIFICATION was done by story card owner and other stakeholders
- Result should be that everyone is able to install and test the code/work relevant to the story, and this just by reading the story card

### Suggestions for documentation

- do not use documentation phase in kanban, documentation is a part executing on the story like any other task (specs, ...)
    - specs/documentation should 20% be done before you start with story and while doing story the specs/docs get completed
