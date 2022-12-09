# Priston-Tale-Installer-for-Linux
This is a script to install `Priston Tale Eu` in Linux. `Steam Deck` is also supported.

## Prerequisits
***!!STEAM DECK USERS CAN SKIP THIS STEP!!***


This software needs to be installed on the system.
* `Flatpak`

*If `Steam` is installed as `Flatpak`*

* Add permissions for `Steam` to access `org.freedesktop.Flatpak` `Session bus`. This can be done easily with `Flatseal`. **Note:** *This removes the sandbox `Steam` runs in*


## Installation

1. Download latest release [here](https://github.com/frlof/Priston-Tale-Installer-for-Linux/releases/download/latest/PristonTaleInstaller.zip).
2. Place downloaded folder in `~/Downloads`
3. Run `Installer` and follow instructions shown in the terminal carefully throughout the install.
4. Add game to `Steam`. Guide is found [here](#add-game-to-steam).

## Add game to Steam

1. Open `Steam` in desktop mode
2. Left click `ADD A GAME` in the bottom left corner
3. Left click `Add a Non-Steam Game...`
4. Choose any program from the list and left click `ADD SELECTED PROGRAMS` (We will reprogram the entry, that is why we can choose ANY program from the list)
5. Right click on the created entry and click `Properties...`
6. Fill the following
    - `Steam` installed with `Flatpak`:
       - *Name*:           `Priston Tale EU`
       - *Target*:         `"/usr/bin/flatpak-spawn"`
       - *Start in*:       `"/usr/bin/"`
       - *Launch options*: `--host flatpak run --command=bottles-cli com.usebottles.bottles run -b "PTCustomEnv" -p "Priston Tale"`
    - `Steam Deck` / Other:
      - *Name*: `Priston Tale EU`
      - *Target*:         `flatpak`
      - *Start in*:       Leave empty
      - *Launch options*: `run --command=bottles-cli com.usebottles.bottles run -b "PTCustomEnv" -p "Priston Tale"`
7.  Play the game!
