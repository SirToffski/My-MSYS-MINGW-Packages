# My-MSYS2-Packages
A collection of custom PKGBUILD's for MSYS2 for packages that are not present in [MSYS2-Packages](https://github.com/msys2/MSYS2-packages) repository.

# Installation
PKGBUILD's are maintained to include all of the `depends` and `makedepends` packages. To build the package, cd into the package folder and build with `makepkg`. For example:

## MSYS2

```bash
$ cd fping/

# To build and install
$ makepkg -sCLfi

# To build only
$ makepkg -sCLf
```

## MINGW

```bash
$ cd pandas/

# To build and install
$ MINGW_ARCH=mingw64 makepkg-mingw -sCLfi

# To build only
$ MINGW_ARCH=mingw64 makepkg-mingw -sCLf
```
