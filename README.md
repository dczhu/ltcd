# ltcd
Less Typing Changing Directory (cd)

![Alt Text](https://github.com/dczhu/ltcd/blob/master/res/cd.gif)

## Introduction
Inspired by [acd_func.sh](http://linuxgazette.net/109/misc/marinov/acd_func.html), ltcd provides the following features to make life easier:

- [x] Global dir listing, which shows recently visited dirs from all terminal tabs/windows.
- [x] Local dir listing, which is local to current shell session.
- [x] Both listings support quick navigation by using j/k (go down/up), numbers, and word searching.
- [x] Global free jumping (e.g. "cd dir" or "cd ar" to go to /path/to/foo/bar/directory/).

## Installation
The scripts (ltcd and cd_utils) are used by sourcing them in ~/.bashrc, and the commands cd/cdrm/cdedit will be ready to use.

## How To Use
* Alt+A or "cd -?" brings up global dir list.
* Alt+Q or "cd --" brings up local dir list.
* "cd $word" for free jumping - 'word' is any part of the **full** path of the dir to go.
* If there is a list, follow the prompt to choose a path to go.

## Note
The files created by ltcd are all at ~/.cd/ for cleanness and debugging purposes.
