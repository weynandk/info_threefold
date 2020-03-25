# specifications & time estimates
![](https://images.unsplash.com/photo-1518775005910-7aa25aa9614a?ixlib=rb-0.3.5&s=475aa3f93a9acaa9d4c05af8d7a7014d&auto=format&fit=crop&w=1433&q=80)

## FR: feature requests are done in appropriate product(code) repo or project repo  (FR)

A Feature request is a feature which should be part of a specific release (product or project or time)
DO NOT PUT SPECIFICATIONS inside the FR

### project or organization related



- e.g. in org_marketing all FR to do with marketing

### code related:

- e.g. in jumpscale8 all FR to do with this product
- FR are linked to a release which is milestone in EE terms e.g. 8.1.0 or linked to roadmap if far away
- FR have links to dir or pages which have the specifications

### FR format

#### links

- make sure all files which have specs   are linked to FR, can be in comment or in main body

- link to all 1 file in same repo

```
- [TestCuisineBuilder.py](../blob/master/tests/tools/cuisine/TestCuisineBuilder.py)
```

- link to all files in dir in same repo

```
- [cuisine_tests](../blob/master/tests/tools/cuisine/)

```

- link to dir or file in remote account/repo

```
- [specs](../../../Incubaid/dev_process/blob/master/specs_format.md)
```

- link to dir or file in remote repo but in same account

```
- [specs](../../dev_process/blob/master/specs_format.md)
```

- what if other branch
   - change 'master' to other branch name in url

#### time info

- can put todo & time info in FR (see below metadata section)
   - this metadata will be additional to metadata as specified in specs where we link to
   
#### todo tables

they are only used to help estimate how much work a specific feature request is, do not put the specs in there

```
- [x] Finish my changes *1 [1h]
- [ ] do something *3 [2h]
- [ ] review code from X [1h]
- [ ] unknown work [5h]
```

- the time mentioned is remaining time so needs to be revisited all the time
- be aware that task lists are never complete !!! always put a last one e.g. unknown work, the total should be total effort for FR

### specs

- specs should always be put in repo where code is developed
- specs can be part of code, suggest to use as much as possible code layouts e.g. the class with methods & todo's & specs are part of that method
- when developing let the specs in, DO NOT remove them, this is good for further checks

### when specific code reviews required

- if specific code review is required can put a todo just for that purpose

### metadata in specs

#### use priorities

```
#TODO: *1 
```

- we support *1 *2 & *3
- *1 is NOW
- *2 is soon, < 1-4 weeks (current sprint)
- *3 is planned in next iteration

#### use links to FR or BUG or STORY in specs

```
(#577)
```

- this can be part of any codeblock or specifications content (e.g. to identify a spec & link to a FR)
- this can be part of a todo in code 

#### use time in specs

- Time format is optional
- Can be in h or days e.g. 4h or 4d 

```
[4d]
```

#### complete example:

```
#TODO *1 do something something [1h] (#577)
```
- this is some task of 1h, ... in this repo (always needs to be in this repo) and this needs to be done ASAP

