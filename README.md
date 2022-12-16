# Zettelmaking

A set of scripts to assist you in creating ["a partner in communication"](http://luhmann.surge.sh/communicating-with-slip-boxes)

## What counts as a note?

Any markdown file (`.md`) with a yaml heading.

```md
---
title: Communicating with Slip Boxes
id: 202212161604 
type:
keywords: []
---
```

To be precise, only the `title:` entry is mandatory.
The `id` is automatically generated by the `zn` script.

## How these scripts might help you?

The "meat" is the script named `zex` (a short for: Zettelkasten Explorer).

Calling `zex` lists all the notes in a given folder.
The list is showed using `fzf`.

Once `fzf` is in the scene, sky is the limit.
You can:
* type a term to filter the list and see only files matching your search (reloads automatically)
* Or hit:
    - `enter`: simply edit selected note(s)
    - `ctrl-b`: search for backlinks to the currently selected note
    - `ctrl-e`: send the note be edited remotely (using nvim session)
    - `ctrl-y`: copy the id of selected note(s)
* Or create anything you want
