# Task

![](images/task.png)

**Task issues can only to be used in [EE Scrum Repo's](https://docs.grid.tf/dividi/efika/src/branch/master/Efika_Agile/EfikaProcess/repositories.md#scrum-repos)**


There is no strict requirement to use tasks in scrum, its something optional.
They can be used if a team feels its useful to cut a story into subtasks because it helps tracking & planning. Tasks are always kept in same repo as where the story has been created !!!

## Format

#### Title: `$taskDescription [4h]` or `$storyname:$taskDescription [4h]`

* Time format is optional
* Can be in h or days e.g. 4h or 4d
* E.g.: `storyx:cuisine start of postgresql does not work [1h]`


## IMPORTANT Remarks

* do not overuse tasks, this leads to abuse very quickly and is not really compatible with scrum or kanban
* scrum is all about the story card owner having a good view on what the story is about and with gut feel & knowledge put best estimate in the title of remaining time \(gutfeel is much more reliable then trying to put tasks in\)
* if you try to describe work by tasks its never correct and at least 50% error because tasks are never complete
* DO NOT describe them too formal !!!!, needs to be a quick placeholder
* DO NOT put content in task \(all this belongs to code repo\)
  * features
  * bugs
  * requirements
  * docs
  * remarks to do with product
* a task is a pure process driven item, do this then, ... NO SPECS

#### Title: `$storyname:$taskDescription [4h]`

* Time format is optional
* Can be in h or days e.g. 4h or 4d
* E.g.: `storyx:cleanup the text for button something [1h]`
* E.g.: `storyx:complete the autotest nr ... [1d]`

### Body:

* Each task is linked to 1 owner who executes the task
* Sometimes its useful that the owner of the task puts a time estimate e.g. \[1h\], this is always the remaining time going from now. This needs to be revisited often

## Shortcut and recommended way how to use tasks.

just use a list of tasks in the story itself and link them to bugs/fr/tickets ...

e.g.

```markdown
- [ ] [crash in server ... on env ...](https://something)
- [x] [fr, nicer UI for page ...](https://something)
- [ ] [don't forget to copy the code to ...](https://something)
- [x] ask feedback to kristof about specs on this task
```

which will be shown as:

- [ ] [crash in server ... on env ...](https://something)
- [x] [fr, nicer UI for page ...](https://something)
- [ ] [don't forget to copy the code to ...](https://something)
- [x] ask feedback to kristof about specs on this task


This is often nicer than having to create subtasks for everything.

