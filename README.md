# ltcd
Less Typing Changing Directory (cd)

Inspired by [acd_func.sh](http://linuxgazette.net/109/misc/marinov/acd_func.html), ltcd provides the following features to make life easier:

- [x] Global dir listing (Alt+A), which shows recently visited dirs from all terminal tabs/windows.
- [x] Local dir listing (Alt+Q), which is local to current shell session.
- [x] Both listings support quick navigation by using j/k (down/up), numbers, and word searching.
- [x] Fuzzy cd globally (e.g. "cd ar" to go to /path/to/foo/bar).

The script is used by sourcing it in a shell rc file like .bashrc, and the command remains the same - cd.

The files created by ltcd are all at ~/.cd/ for cleanness and debugging purposes.

