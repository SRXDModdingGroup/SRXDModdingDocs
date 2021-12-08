# Installation

## Automatic Installation

1. Go to [https://github.com/SRXDModdingGroup/SRXDBepInExInstaller/releases/latest/](https://github.com/SRXDModdingGroup/SRXDBepInExInstaller/releases/latest/) and download the installer for your operating system.
2. Run the installer.
3. Put your mods in the `Spin Rhythm\BepInEx\plugins` folder.

## Manual Installation

If you get the error "failed to execute script srxdbepinexinstallerui" or installer not responding, try this method below to get it installed:
### 1. Installing BepInEx
1. Navigate to `Steam\steamapps\common\Spin Rhythm`
2. Go to [https://builds.bepis.io/projects/bepinex_be](https://builds.bepis.io/projects/bepinex_be), scroll down to your preferred version and get the one that says "BepInEx Unity IL2CPP for Windows x64 Machines"
3. Extract the zip into your `Spin Rhythm` folder (`Steam\steamapps\common\Spin Rhythm`).

### Optional (Only Do these Steps If You are Installing Versions 378 or Lower!)
1. Go into the "BepInEx" folder that is now in your `Spin Rhythm` folder.
2. Create a folder naned `unity-libs` inside of the BepInEx folder
3. Go to [https://github.com/LavaGang/Unity-Runtime-Libraries/raw/master/2020.1.15.zip](https://github.com/LavaGang/Unity-Runtime-Libraries/raw/master/2020.1.15.zip)
3. Download the zip and extract it into the just created "unity-libs" folder

### 2. Finalizing
1. Now navigate to `Spin Rhythm\BepInEx`
2. Create a `plugins` folder inside the `BepInEx` folder
3. Put your mods in the `Spin Rhythm\BepInEx\plugins` folder.

## Notes for Linux and Mac Users

__If you are on Linux or Mac, remember to add `winhttp` to the wine configuration overrides. Otherwise, BepInEx may not start with the game.__

Here's how to do that:
### Proton on Linux Users (Make sure Winetricks is installed)

```shell
# Install pipx
## Arch Linux:
sudo pacman -S python-pip python-pipx python-setuptools python-virtualenv
## Debian linux
sudo apt install python3-pip python3-setuptools python3-venv pipx
## Fedora Linux
sudo dnf install python3-pip python3-setuptools python3-libs pipx

# Use pipx to install Protontricks (you might have to restart your terminal)
pipx install protontricks
# After install, enable desktop integration
protontricks-desktop-install

# Run protontricks
protontricks --gui
## Select Spin Rhythm XD from the list of games
## Select the default wineprefix
## Run winecfg
```

### Then Navigate to the Libraries Tab
![Add winhttp.dll](assets/winhttp_add.gif)
