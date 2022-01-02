# This is my setup for dmenu
## Get Started
If you want to apply certain changes to your `config.h`, apply that to `config.def.h` instead. Then run
```
$ sudo cp config.def.h config.h
$ sudo make clean install
```
This ensures that future patches won't overwrite the changes in your `config.h` since what those patches do is that they patch the `config.def.h` then copy that to `config.h` (basically the steps that we did).<br />
To apply the patch, run:
```
$ sudo cp config.def.h config.h
$ patch -p1 < <patch>
```
> Read this [documentation](https://suckless.org/hacking/) by suckless on how to apply patches.

## Patches applied (in order)
- [border](https://tools.suckless.org/dmenu/patches/border/dmenu-border-4.9.diff)
- [case-insensitive](https://tools.suckless.org/dmenu/patches/case-insensitive/dmenu-caseinsensitive-20200523-db6093f.diff)
- [fuzzyhighlight](https://tools.suckless.org/dmenu/patches/fuzzyhighlight/dmenu-fuzzyhighlight-4.9.diff)
- [fuzzymatch](https://tools.suckless.org/dmenu/patches/fuzzymatch/dmenu-fuzzymatch-4.9.diff)
- [center](https://tools.suckless.org/dmenu/patches/center/dmenu-center-20200111-8cd37e1.diff)
- [alpha](https://tools.suckless.org/dmenu/patches/alpha/dmenu-alpha-20210605-1a13d04.diff)
- [lineheight](https://tools.suckless.org/dmenu/patches/line-height/dmenu-lineheight-5.0.diff)

