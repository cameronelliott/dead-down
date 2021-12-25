
<!-- omit in toc -->
# dead-down 


Dead-simple page-load-time Markdown to HTML website creation tool. Uses MarkedJS, and PrismJS

<!-- omit in toc -->
## Table of Contents

- [Another Example](#another-example)
- [Basic Directions](#basic-directions)
  - [Methods to get these files into `./dead-down/*`](#methods-to-get-these-files-into-dead-down)
- [Updating PrismJS](#updating-prismjs)

## Another Example

Can be found [here](example1/index.html)

## Basic Directions

1. Drop the files from this repo under `dead-down`, see below for methods.
2. Create a directory. This will be the URL for the new file.
3. `$ mkdir foo`
4. Create a file 'readme.md' under the directory.
5. `$ echo # New Doc >foo/readme.md`
6. Now create a symbolic link under the new directory.
7. The command is `ln -s dead-down/index.html foo/index.html`
8. Edit the content to get it to where you need `foo/readme.md` 

### Methods to get these files into `./dead-down/*`
1. Unzip these files into `dead-down`
2. Add this repo as a git submodule under `dead-down`
3. Clone this repo as a regular git repo under `dead-down`

Get a zip, and unzip it.
```bash
curl http://github.com/cameronelliott/dead-down | unzip -v
```

Add as a submodule if you like that way
```bash
git submodule add http://github.com/cameronelliott/dead-down
```

Clone as regular git repo
```bash
git clone http://github.com/cameronelliott/dead-down
```

## Updating PrismJS

If you open up the file prism.js, the first line shows the url which
was used to download the .js and .css files.
