# info_threefold

Welcome to the ThreeFold Ecosystem Wiki.
Here is where you'll find all info on anything related to ThreeFold.

Things like:
- The Token
- The Grid
- 3Bot
- ThreeFold Tech
- And more.

If you have any input, would like to see additions, or a cool idea feel free to list an issue and we'll make sure to try and get it in there.

If you need any support please visit [our website](https://www.threefold.io) and use the chat widget in the bottom right of your screen.
Our team will answer your questions as soon as possible.

Now go explore our wiki's.

#### Editing in the wikis

- all md files are under src/docs directory, please make sure you get all your changes there.

### MDBOOK HOW TO :-

after changing any file, build has to be run 
cd into the repo directory then run this command :-

```
mdbook build info_threefold -d docs

```

 - changeing the title :- 
    - from book.toml file
  ```
  title = "Threefold Foundation"
  ```
  
 - changing the default theme
    - from book.toml file
```
default-theme = "Rust"
```

- Runing mdbook server :- 

**use -p for specifying port number**

cd into the repo directory then run this command :-
```
mdbook serve info_threefold -n 0.0.0.0
```


- Sidbar foldable setting, enabled by adding this part to book.toml file :-

```
[output.html.fold]
enable = true
level = 0

```
