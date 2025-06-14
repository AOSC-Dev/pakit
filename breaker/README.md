Breaker
===

Python script to generate rebuild lists and PKGBREAK metadata, and to bump REL.

Usage
---

```
usage: breaker [-h] [-a] [-r] [-p] [-s SOREVDEPS [SOREVDEPS ...]] [-b] [-d] [-e EXCLUDE [EXCLUDE ...]] [-i INCLUDE [INCLUDE ...]] package

Breaker make bumping shared library easy

positional arguments:
  package               Package name to update

options:
  -h, --help            show this help message and exit
  -a, --alldeps         Include all reverse dependencies, not only library reverse dependencies
  -r, --rebuilds        Generate groups/xxx-rebuilds
  -p, --pkgbreak        Generate PKGBREAK
  -s SOREVDEPS [SOREVDEPS ...], --sorevdeps SOREVDEPS [SOREVDEPS ...]
                        Use specific soname to generate reverse dependencies
  -b, --bump            Bump dependencies one in a git commit
  -d, --debug           Enable debug message
  -e EXCLUDE [EXCLUDE ...], --exclude EXCLUDE [EXCLUDE ...]
                        Exclude packages from reverse dependencies
  -i INCLUDE [INCLUDE ...], --include INCLUDE [INCLUDE ...]
                        Add extra packages to reverse dependencies
```
