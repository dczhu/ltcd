# ltcd
Less Typing Changing Directory (cd)

![Alt Text](https://github.com/dczhu/ltcd/blob/master/res/cd.gif)

## Introduction
Inspired by [acd_func.sh](http://linuxgazette.net/109/misc/marinov/acd_func.html), ltcd provides the following features to make life easier:

- [x] Global dir listing, which shows recently visited dirs from all terminal tabs/windows.
- [x] Local dir listing, which is local to current shell session.
- [x] Both listings support quick navigation by using j/k (go down/up), numbers, and word searching.
- [x] Global free jumping (e.g. `cd dir` or `cd ar` to go to /path/to/foo/bar/directory/).

## Installation
In ~/.bashrc:
1. source the script [h](https://github.com/dczhu/mch/blob/master/h), which is a multi-color pattern highlighter.
2. source the script [cxpgrep](https://github.com/dczhu/cxpgrep/blob/master/cxpgrep), which is an exteded grep command that uses the command `h`.
3. source the script [ltcd](https://github.com/dczhu/ltcd/blob/master/ltcd), and the commands `cd`/`cdrm`/`cdedit` will be ready for use. The script ltcd uses the command `cxpgrep`.

## Usage
* Alt+A or `cd -?` brings up global dir list.
* Alt+Q or `cd --` brings up local dir list.
* `cd $word` for free jumping - 'word' is any part of the **FULL** path of the dir to go.
* If there is a list, follow the prompt to choose a path to go.
  - [x] Use the keys j/k to navigate down/up the entries - A single backspace will remove the whole line - Be fast!
  - [x] Type a number to select a specific entry (0 or empty means staying put).
  - [x] Start a search by typing / and then the word.
* This code is intended to be compatible with the original cd command - e.g. `cd -` brings you back to the previous dir.
* Run `cdrm` to remove invalid entries in global bookkeeping. Invalid entries are removed/renamed/inaccessible dirs.
* Run `cdedit` in case you want to edit the global bookkeeping. For example, if you feel some dirs with "tmp" in the path name are not useful to stay in the record, you can manually remove them with this command.

## Note
The files created by ltcd are all at ~/.cd/ for cleanness and debugging purposes.

## Releases
* 1.0
  - [x] First working code

## License
This software (ltcd) is distributed under the [MIT license](https://github.com/dczhu/ltcd/blob/master/LICENSE).
