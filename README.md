# MacSetup
This repo contains a list of steps to be performed duing a mac setup for software developer
## Homebrew
This step on your mac is essential to other dev dependency installations
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
## Iterm
1. Install the terminal from here: ```brew install --cask iterm2```
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
10. I am using powerlevel10k. Install it using: ```git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k```

## Git
1. Install git : ```brew install git```
2. Generate ssh-key: ```ssh-keygen -t ed25519 -C "your_email@example.com"```
3. Start the ssh-agent in the background: ```eval "$(ssh-agent -s)"```
4. If file doesn't exist create it: ```touch ~/.ssh/config```
5. Modify the contents of the file
   ```
   Host github.com
   AddKeysToAgent yes
   UseKeychain yes
   IdentityFile ~/.ssh/id_ed25519    # Change this to path in your case
   ```
6. Add your SSH private key to the ssh-agent : ```ssh-add --apple-use-keychain ~/.ssh/id_ed25519```
7. Copy & paste to GitHub profile > settings > SSH & GPG Keys, ‘New SSH Key’. Add to profile
4. Configure git cli
```
   git config --global user.email “you@example.com” 
   git config --global user.name “Your Name”
```

## JAVA
1. Install java: ```brew install openjdk@17```

## Node and npm
1. Using nvm to install node and npm to manage multiple versions of node.
2. Intalling nvm:```curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash```
3. Restart terminal
4. Intall node,npm : ``` nvm install node ```


## Editors
### VSCode (Using it for node/js/react programming)
1. Install it from here: https://code.visualstudio.com/
2. Extensions
   * Material Theme
### Intellij
1. Install: https://www.jetbrains.com/idea/download/?section=mac



