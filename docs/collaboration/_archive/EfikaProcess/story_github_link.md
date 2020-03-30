
# automatic linking between tasks/bugs/fr and stories

To make our life easy we have created a tool which links bugs/tasks/feature requests to stories automatically. For that we use the task format feature in markdown.


- link stories to bugs or feature requests on github
- the stories and tasks are only on our [EE Scrum Repo's](https://docs.grid.tf/dividi/efika/src/branch/master/Efika_Agile/EfikaProcess/repositories.md#scrum-repos)
- the bugs/fr are only on github

## bug/fr format on github

title

```
$storyname: ... rest of bug/fr
```

## task format on [EE Scrum Repo's](https://docs.grid.tf/dividi/efika/src/branch/master/Efika_Agile/EfikaProcess/repositories.md#scrum-repos)

title

```
$storyname: ... rest of bug/fr
```

## story format on [EE Scrum Repo's](https://docs.grid.tf/dividi/efika/src/branch/master/Efika_Agile/EfikaProcess/repositories.md#scrum-repos)

title

```
$story_description $hoursoptional ($storyname)
```

## 2 examples

- see https://docs.greenitglobe.com/gig/org_development/issues/19
- see https://github.com/zero-os/0-templates/issues/76

## The resulting task table is as follows

format as used in story

```markdown

## bugs/fr

- [x] [[$bug/fr_description $optional_hours]($link_to_the_issue_on_github)
- [] [[$bug/fr_description $optional_hours]($link_to_the_issue_on_github)

## tasks 

- [ ] [$taskdescription $optional_hours]($link_to_the_issue_on_EE)
- [ ] [$taskdescription $optional_hours]($link_to_the_issue_on_EE)
- ...

```

## but reference to story in bug/fr/task

do this by using following format

```markdown

## stories

- [ ] [$storydescription]($link_to_the_story_on_EE)
- [ ] [$storydescription]($link_to_the_story_on_EE)

```

## how

- a tool run by someone who has access on github and the EE.
- this tool will walk over all specified repo's on github & EE
- tool will find stories which has name defined in ()
- tool will find issues which have $name: ... in title if link found to story above the links are made in tables.

remarks

- need to make sure that broken links are removed, so only active links are there


- 