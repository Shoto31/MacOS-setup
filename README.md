# MacOS-setup

## This are all the things I do to setup my Mac

### Install Homebrew

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### Install alacritty
```
brew install --cask alacritty
```

### Install and COnfigure zsh and oh-my-zsh

```
brew install zsh
```
Set zsh as the default shell
```
chsh -s /opt/homebrew/bin/zsh
```
Now to install oh-my-zsh (themes)

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
brew install spaceship  # Install the spaceship theme
echo "source $(brew --prefix)/opt/spaceship/spaceship.zsh" >>! ~/.zshrc # add prompt initialization to your .zshrc
```
