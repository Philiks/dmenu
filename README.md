# This is my setup for dmenu
## Get Started
If you want to apply certain changes to your `config.h`, apply that to `config.def.h` instead. Then run
```
$ cp config.def.h config.h
$ sudo make clean install
```
This ensures that future patches won't overwrite the changes in your `config.h` since what those patches do is that they patch the `config.def.h` then copy that to `config.h` (basically the steps that we did).<br />
To apply the patch, run:
```
$ patch -p1 < <patch>
```
> Read this [documentation](https://suckless.org/hacking/) by suckless on how to apply patches.

## Patches applied 

