# Problem

The `cycler=0.10` package from `conda-forge` installs as a [Python Egg][egg],
with the following files installed to `site-packages`:

    cycler.pth
    cycler-0.10.0-py2.7.egg

However, py2exe [_"...does not support including Python eggs in its
binaries..."_][noegg].

# Workaround

This recipe installs `cycler` from the Python Package Index, which installs as
a regular package (i.e., not an egg).


[egg]: https://wiki.python.org/moin/egg
[noegg]: http://python101.pythonlibrary.org/chapter40_py2exe.html#creating-an-advanced-setup-py-file
