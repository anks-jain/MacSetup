# MacSetup
This repo contains a list of steps to be performed duing a mac setup for software developer
## Homebrew
This step on your mac is essential to other dev dependency installations
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
## Git
```
brew install git
```
### Copy your ssh key to github
1. ssh-keygeen
2. View key: ~/.ssh/id_rsa.pub
3. Copy & paste to GitHub profile > settings > SSH & GPG Keys, ‘New SSH Key’. Add to profile
4. Configure git cli
  * git config --global user.email “you@example.com” 
  * git config --global user.name “Your Name”
## Editors
1. VSCode
2. Sublime
3. Intellij
