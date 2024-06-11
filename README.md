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
<details>
<summary><h3>Shell</h3></summary>
  
- Install and Configure zsh and oh-my-zsh

```
brew install zsh
```

- Set zsh as the default shell

```
chsh -s /opt/homebrew/bin/zsh
```

- Now to install oh-my-zsh (themes)

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
<details>
  <summary><h3>Spaceship Prompt</h3></summary>
    
- Install the spaceship theme
  
```
brew install spaceship  
```

- Add prompt initialization to your .zshrc
 
```
echo "source $(brew --prefix)/opt/spaceship/spaceship.zsh" >>! ~/.zshrc
```

</details>

- Plugins that I use
```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```
- After this simply add the following to you "~/.zshrc" file
```
plugins=(git zsh-autosuggestions zsh-syntax-highlighting web-search)
```
### Then run in your terminal
```
source ~/.zshrc
```
</details>
