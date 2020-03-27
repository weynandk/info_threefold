# Trello Usage

![@https://images.unsplash.com/photo-1494074734099-c4ec0c45687a?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=f18b2bf25abbaeddbe5ea1f9dae1ff85&auto=format&fit=crop&w=1950&q=80](trello_usage.jpeg)


**Make sure every board is defined in** the [circles document](/circles/readme.md)

REMARK: if you don't agree with anything on this document then please create Issue in this repo so we can discuss.
We highly appreciate you don't deviate from simple rules below.

DO NOT USE TRELLO FOR ISSUES/STORIES/FEATURE REQUESTS WHICH HAVE TO DO WITH CONTENT THEY BELONG ON GITHUB [see here](/collaboration/Github_content_rules.md)

## The Info Card

Example https://trello.com/c/o8VWFzcH/23-info

An info card should be created on each trello board containing all the links to the info related to this board.

E.g. links to circle page, link to Gdrive, link to other relevant trello boards, ...
e.g. info about timing (needed for e.g. trello roadmap board)

## Different types of trello boards


### Funnel board

- Storyboard name: $teamname_funnel_$region or $teamname_funnel if no region e.g. tfgrid_funnel_africa
   - teamname is without _
- Swimlanes / columns
   - New          : first contact, validating opportunity
   - Interested   
   - Confirmed    : email or oral confirmation that they want to do the deal
   - Negotiation  : working on the details, contract stage sits in here
   - Won          : all docs done, waiting for e.g. payment, delivery, ...
   - Idea         : should we contact & continue with the prospect
- When a story is won & paid > archive. When a story lost > archive

Use labels for:

- Urgency e.g. red (when more urgent just move to top of list, red/orange is to promote even more)
- Named labels can be used for e.g. region, ...  (free to select)
- There needs to be a chat attached to each funnel board

### Stories board

- Stories are about groups of people working together that have regular meetings
   - boards are used to organize work over defined intervals
   - do not copy info from funnel or roadmap board
- Storyboard name: $teamname_stories_$name e.g. tftoken_stories_promotion
   - teamname is without _
- [How to write a story](/collaboration/stories.md)
- Board owner
   - calls meetings when required
   - communicate with board members to help them with communication, ...
- Story owners
   - owns the story and makes sure is executed in time & done following all requirements
- Swimlanes (follow this order)
  - new: not approved to work on yet
  - this_week
  - question_blocking
  - this_month
  - this_quarter
  - verification (needs to stay in here till at least board owner approves)
  - future
- When a story is done or no longer valid > archive
- Stories can have tokens attached to them:
   - create checklist call: token_bounty add people on there with token amount & lockup period e.g. 10000_oct_19
- There needs to be a chat attached to each stories board
- Labels (goal is to not have many labels on the stories)
   - critical: can only be used in this_week, means need to be looked at TODAY, its critical means, resolve today
   - major: can only use in this_week or this_month is to give prio to a card
   - minor: means its ok if it gets postponed to next iteration (do not overuse !)
   - info (blue): is an info card, stays there for ever, only 1 per board !!!
- Use a deadline per week/month to inforce timing, trello will show when it gets dangerous
- when stories are done (means out of verification), just archive them 

### Roadmap board

Roadmaps are about content (feature requests, issues, ...) which need to be executed in a certain version of a delivery of a product or e.g. a website

- storyboard name: $teamname_roadmap_$name e.g. tftoken_roadmap_web
   - teamname is without _
   - web would be for wiki & websites
   - e.g. tftech_roadmap_archive
- swimlanes
   - $version
   - for the first to be delivered version use $version/$version_question/$version_done 
       - in other words the next version to be delivered has 3 swimlanes attached to it
   - do not have more than 3 versions active
   - the last one = 'future'
 - the focus here is on the content of the feature, issue and the version its not a story or a task !!!
 - the story owner = makes sure that the feature will be done in the right version
 - there needs to be a chat attached to each roadmap
 
