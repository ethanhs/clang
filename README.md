# Clang Python bindings

These are *unofficial* Python bindings to clang as taken from the clang source
tree, packaged for installation from PyPi. 

You *must* install clang for this library to work. You can usually install it
from your distribution's package manager or from
http://releases.llvm.org/download.html.

After installing clang, you should be able to

```
pip install clang
```

In the interest of keep things simple, this package will have the same version
numbers as the clang release they were taken from.

## Why does this exist?

Most Linux distributions' clang package already contain the Python
bindings, so no more work is needed. However, on Windows, installing the
bindings along with clang is not feasible, so this package was created.


This package was originally maintained by @trolldbois, huge thanks to him for
his many years of work on it!

### Tests note

In the interest of making my life easier, I have added a pytest.ini and
modified the tests to run on Windows with a patch I upstreamed to LLVM
https://reviews.llvm.org/D47864