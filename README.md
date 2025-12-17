# F-100D Manual

[View Here](https://f100d.manuals.gd.sloanphillippi.com/)

The F-100D manual is written in markdown. You can find a [cheatsheet here](https://github.com/adam-p/markdown-here/wiki/markdown-cheatsheet). Try to avoid using complicated markdown features because we need to be able to render the manual in the imgui if/when we do the in-game manual project.

![test-image](plane.png)

Be sure to make use of links wherever possible to make it easy to navigate and put images where you would expect even if you don't have an image yet.

The exact structure is to be discussed.

![gif-test](src/Weapon_System/gunsight.gif)

## Install

`pip install mkdocs`

`pip install mkdocs-print-site-plugin`

## View

`mkdocs serve`

## Build

`mkdocs build`

> Note: for venv mkdocs can be run with `python -m mkodcs ...`

Output html file is in site/print_page, material theme should be used for links to work.
