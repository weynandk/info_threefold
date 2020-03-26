# How to edit

We integrated a feature in 3bot that allows you to have a code editor in the browser so you don't have to go anywhere else, only from your browser, you edit, preview, change and apply into git repository

## Wiki syntax
Wikis are using the popular markdown format and "macros" for more advanced use cases. Visit [wikis](./wikis.md) tab for more info on that.

## CodeServer 

In 3bot admin dashboard you can access it on http://localhost:7000/admin

![](./images/admindashboard.png)

you can then go to our online code editor `CodeServer` in the sidebar codeserver http://localhost:7000/admin/#!/main/codeserver and see something like

![codeserver](./images/codeserver.png)
Here you can edit files easily and you can preview the markdown files as well

### Terminal

![codeserverterminal](./images/codeserverterminal.png)
You have a full access to the terminal as well so you can execute commands or manipulate git as well


### Committing changes

After checking your changes in the [wikis](./wikis) tab


using the terminal:

- first make sure you have the `info_threefold` wiki if you don't just execute `jsx wiki-load` check [wikis.md](./wikis.md) for more info on loading wikis
- go to `/sandbox/code/github/threefoldfoundation/info_threefold` using the command `cd /sandbox/code/github/threefoldfoundation/info_threefold`

- `git add .`
- `git commit -m "suitable commit message describing the changes"`
- `git push`



