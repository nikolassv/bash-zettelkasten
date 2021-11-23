# bash-zettelkasten

A collection of bash-scripts for organizing a plaintext zettelkasten.

[![License: GPL](https://img.shields.io/badge/license-GPL-blue)](LICENSE)

## Installation

This repository does only contain some bash scripts. You may _install_ it by cloning it locally and adding the `bin` directory to your `PATH` environment variable.

Just add this line to your `.bashrc`:

```bash
export PATH="path-to-the-cloned-repository/bin/:$PATH"
```


## How to use it

Each note in your zettelkasten is a plaintext file. You may create and edit them with whatever tool you like. The names of the files are not important. You may give them meaningfull as well as random names.

You can add tags to your notes as words prepended with a hash sign (#...). Each note can have as many tags as you like. Beside tags you can use any markup you like in notes. Just be aware that every string prepended by a hash sign will be interpreted as a note.

The bash scripts in this repository act as simple tools for organizing your notes:

```
zk-tags                         # list all tags
zk-find tag1 tag2 tag2          # show all notes containing tag1, tag2, and tag3
zk-find tag1 -tag2              # show all notes containing tag1 but not tag2
zk-files-find tag1 tag2 -tag3   # list all files containing tag1 and tag2 but not tag3
```

## Autocompletion

To add autocompletion to `zk-find` source the file `bin/_zk-autocomplete` in your `.bashrc` file:

```bash
source path-to-the-cloned-repository/bin/_zk-autocomplete
```

## Links

* [Wikipedia: Zettelkasten](https://en.wikipedia.org/wiki/Zettelkasten)
* [Zettelkasten.de - Getting Started](https://zettelkasten.de/posts/overview/) - Several useful ressources for getting started with a zettelkasten
