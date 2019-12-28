# EyeDevelop's DotFiles
![Some image of dotfiles I found](img/dotfiles.png)

## Installation
### Dependencies
This script will install all the dependencies it needs.
Do make sure yay is installed, otherwise these packages
cannot be installed.

### Actual installing!
**Warning:** Please look at the code before you execute blindly.

The helper install script:
```bash
./install.py --help
```

To install all the dotfiles in the user's home directory:
```bash
./install.py -d ~/ -m all
```

You can look at what can be installed by looking in the 'installers' folder.

## Updating
> "Because re-installation sucks."

**Same warning applies as listed above.**

Just use the Update helper script.
```bash
./update.py --help
```

To update all the dotfiles in the user's home directory:
```bash
./update.py -d ~/ -m all
```

As you can see, the update helper uses the exact same syntax as the installer.

## Useful commands/links:
- [Trackpoint config](https://askubuntu.com/questions/37824/what-is-the-best-way-to-configure-a-thinkpads-trackpoint)
- [Trackpad config](https://cravencode.com/post/essentials/enable-tap-to-click-in-i3wm/)
```
echo 65 | sudo tee /sys/devices/platform/i8042/serio1/serio2/sensitivity # Trackpoint sensitivity
```

## Side notes
Sometimes, durring installation, some programs such as spotify, betterlockscreen, etc. fail do download.
A solution to this could be to install them again:
`yay -S betterlockscreen spotify`
