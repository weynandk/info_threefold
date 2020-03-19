## Roles & Responsibilities Product Development / Project Management

![](images/roles.png)

Different roles as used in Efika Methodology.

### Scrum Master

* Owns a team of people working on one or more stories
* Scrum Lead needs to make sure
  * People understand Scrum and our Agile principles
  * People are coached
  * People improve in their career
  * People are happy in their job and are motivated
  * Eliminate all blockers which people might experience
* Scrum leads are often also story owners \(of X nr of stories\)
* Scrum teams have their own repo: e.g. `org_development_$scrumTeamname`
  * or e.g. `org_marketing` if not related to a product
* A Scrum Master is not a controller ! its a person at service of his team. A Scrum Master = a coach.

### Project Owner

* Responsible for a `proj_$customer_$proj` or `proj_$company_$proj` repo

* Responsibility

  * Define milestones
  * Make sure the repo is clean
  * Verify / Check all stories as defined in repo \(guarantees quality, priorities, communication around it, ...\)
  * Work with product owners to make sure you get the features as required.
  * Work with Scrum Masters to plan the works as required (create required Story Cards)
  * Organize project meetings \(see [Meetings](meetings.md)\)
  * A Project owner does not own people, its a person who coordinates around a project. 
  * The only way how a project owner can get things done is by creating story cards & work with 1 or more scrum teams.

* There is only one project manager per repo

* in readme.md of repo there needs to be clear definition about project & owner & contact info

* They use their telegram group: e.g. `$company_proj_$customer_$proj`

### Product Owner

* Responsible for a EE account/organization e.g. jumpscale

  * They use the home repo to define the structure in the account

* Important to structure the accounts/organizations well so they represent a product

* Responsibility

  * Define milestones=versions on the repo's, make sure they are consistent
  * Make sure the repos in the account/organization are clean
  * Make sure everyone using the repo's behave well
    * proper defined bugs/fr
    * proper branching
  * Work with Project/Product Managers & other stakeholders to make sure the repo structure is ok.
  * Organize product meetings \(PM\) \(see [Meetings](meetings.md)

* There can be more than 1 owner per repo, but try to only have 1.

* The home repo is important to organize the full account/organization.

* They use their telegram group: `$company_product_$name`

### Product Manager

* Owns product from a go2market/commercial/marketing perspective.
* Defines roadmap.
* Creates/owns lots of story cards (for the product parts)
* Organizes stakeholder meetings.
* Owns one or more repo's \(prod\_...\) on EE

### Story owner \(product related\)

* Main responsibilities:
  * Story card is developed in time
  * Story card is clear and understood by all required
  * Requirements for the card are met
  * Done means done! \(see [Agile Principles](../agileprinciples/readme.md)\)
  * Communicate to product owners about the card
  * Organize story meetup in order to talk with people contributing to the story, follow-up on progress
  * Define tasks that need to be delivered to deliver the story card

#### What are the duties of a story owner

* Format of story is fully compliant
* Content of story is properly done \(description, requirements, ...\)
  * Requirements are clear
  * All involved people understand the story properly
* Be part of product meetings \(PM's\), give info:
  * How far are we
  * What are the blockers
  * What is planned now
  * Do this by commenting on story card
* Escalate to product owner\(s\) & Scrum Owner when
  * Story has delay
  * There are questions
  * Do this by comments and also use relevant \(e.g. Telegram\) communication group to escalate to appropriate people
* Guarantee Story gets done which means
  * Code/Work is complete
    * Features are in line with requirements
  * Tests (for product related) are good enough
  * Good documentation that can be understood also by someone who did not work on the story
  * On VERIFICATION phase the pull request is properly merged in \(after VERIFICATION of course\)
  * Code  (for product related) can easily be build and installed by anyone
  * Everyone relevant understands story is done and declare victory!

### Stakeholder

* Anybody who has something to loose or win by the acceptance/progress on a story card
* Stakeholder main responsibility is to be part of product stakeholder meeting \(PSM\)
* This is a very generic definition & can be quite broad.
