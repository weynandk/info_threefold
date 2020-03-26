# Wikis

In 3bot admin dashboard you can access it on [localhost:7000/admin](localhost:7000/admin)

![](./images/admindashboard.png)

You can then go wikis tab in the sidebar
![](./images/wikis.png)

As you can see, you will find a listing of all loaded wikis where you can 

- view the wiki with `View` button.
- pull the wiki changes from git repository in case other people are working on that as well using `Pull` button.
- reload the wiki changes you did locally using `Reload` button.

## How to load a wiki

From the terminal -mentioned in [editing](./editing.md)- execute `jsx wiki-load -u https://github.com/threefoldtech/jumpscaleX_threebot/tree/development/docs/wikis/examples/docs -n examples -f`


#### Options you can use
- -u or --url: docsite url
- -n or --name: wiki name to be used in the dashboard
- -f to load in foreground if not it'll use load it in the background
- -r or --reset" reset git revision and process all files

## How to load info_threefold wikis

From the terminal -mentioned in [editing](./editing.md)- execute `jsx wiki-load -u https://github.com/threefoldfoundation/info_threefold/blob/development/docs -n info_threefold -f`




## How to write 

### Tooling
You only need your webbrowser, check [editing](./editing.md)

### Syntax

Wikis format is a superset of markdown. so all the [markdown syntax](https://www.markdownguide.org/basic-syntax/) works + more advanced features using "macros"

- [Links](./links.md)
- [Macros](./macro/README.md)
- [Inline HTML](./inline_html)