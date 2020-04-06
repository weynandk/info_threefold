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

### how to install mdbook

OSX:

```bash
brew install mdbook
```

### get the documents (content)

```bash
mkdir -p ~/code/github/threefoldfoundation
cd ~/code/github/threefoldfoundation
clone https://github.com/threefoldfoundation/info_threefold/ -b development
```

### use mdbook locally

```bash
cd ~/code/github/threefoldfoundation/info_threefold
#will open local browser
mdbook serve -n 0.0.0.0 -o
```

### Editing the wikis

- all md files are under src/docs directory, please make sure you get all your changes there.
- to make link in md file to open in new tab use this 

#### tips and trics

```
<a href="http://example.com/" target="_blank">Hello, world!</a>
```

