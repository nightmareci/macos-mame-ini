# Template mame.ini files for macOS MAME
Copy one of the INI files to the `.mame` folder in your home folder:
```sh
mkdir ~/.mame
cp ..._mame.ini ~/.mame/mame.ini
```
**You must copy it into `~/.mame` exactly as `mame.ini` or it won't work!**

The INI file you should use depends on how you installed MAME:
* `x86_64_homebrew_mame.ini`: Use if you have an Intel Mac and installed MAME via [Homebrew](https://brew.sh/).
* `arm64_homebrew_mame.ini`: Use if you have an Apple Silicon Mac (M1 or newer) and installed MAME via [Homebrew](https://brew.sh/).
* `macports_mame.ini`: Use if you installed MAME via [MacPorts](https://www.macports.org/). Works for all Macs.

A few settings have been adjusted to make MAME work well enough on macOS, like setting the `video` option to `accel`, which makes performance a lot better than the default `auto` setting, which doesn't even run full speed on M1 Mac mini. And `lowlatency` has been enabled, because why not?
