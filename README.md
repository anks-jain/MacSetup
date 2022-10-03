# MacSetup
This repo contains a list of steps to be performed duing a mac setup for software developer
## Homebrew
This step on your mac is essential to other dev dependency installations
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
## Iterm
1. Download and install the terminal from here: https://iterm2.com/
2. Install "Oh-my-zsh": ```sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"```
3. Download Material Design Colours
```
cd Downloads
curl -O https://raw.githubusercontent.com/MartinSeeler/iterm2-material-design/master/material-design-colors.itermcolors
```
4. Go to iTerm2 > Preferences > Profiles > Colors Tab
5. Click Color Presets… at the bottom right
6. Click Import…
7. Select the material-design-colors.itermcolors file
8. Select the material-design-colors from Load Presets…
9. Do tweaks according to your choice.
10. I am using theme "easterwood"

## Git
1. Install git : ```brew install git```
2. Generate ssh-key: ```ssh-keygen```
2. View key: ```~/.ssh/id_rsa.pub```
3. Copy & paste to GitHub profile > settings > SSH & GPG Keys, ‘New SSH Key’. Add to profile
4. Configure git cli
```
   git config --global user.email “you@example.com” 
   git config --global user.name “Your Name”
```
## Editors
1. VSCode
2. Sublime
3. Intellij
