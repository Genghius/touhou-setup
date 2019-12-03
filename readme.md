# Touhou Setup

This script will create a .desktop launcher for your touhou games.

## Install

```
git clone https://github.com/eylles/touhou-setup
cd touhou-setup
chmod +x ./install.sh
./install.sh
```
The install script will locate the tuhustp scripr in the $HOME/.local/bin/ directory and add it to PATH in .bashrc IF it ain't already added to PATH in your system, if you have a different dedicated scripts directory already added to PATH just go there in a terminal and run:
```wget https://raw.githubusercontent.com/eylles/touhou-setup/master/tuhustp```

## How To Use

just open a terminal and run the script
```
$ tuhustp
```
the script will find all your official touhou pc games and will proceed to create launchers for them
the script can also create the .png icons for the games if you don't have them, just install icoutils and re-run the script

icoutils is present in the official repos for most distros
for ubuntu/debian and derivates: ```$ sudo apt isntall icoutils```
for arch and derivates: ```$ sudo pacman -S icoutils```


## Okay but why?

- opening a file explorer just to play your games is a hassle when you can simply have an icon in your desktop or app menu that will run the game with a click
- manually creating a .desktop launcher is also a hassle if you have more than one game you play
- with some games if the command to execute in the .desktop looks like this ```Exec= wine "/path/to/your/game/th.exe"``` the game will start without music