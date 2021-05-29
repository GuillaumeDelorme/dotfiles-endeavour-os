# Dotfiles and things to do after fresh EndeavourOS install

## Update and install usefull apps

```sh
yay
yay -S --needed \
  blender \
  brave-bin \
  cozy-desktop \
  discord \
  docker \
  gimp \
  inkscape \
  keeweb-desktop-bin \
  libreoffice-fresh \
  lolcat \
  molotov \
  nvm \
  ruby-colorls \
  slack-desktop \
  steam \
  tilix \
  visual-studio-code-bin \
  ytmdesktop-bin \
  zsh \
```

## ZSH

- Install a nerd font : https://www.nerdfonts.com/font-downloads (I use "Fira Code Bold")
- Choose the nerd font in your terminal
- Install oh my zsh : https://ohmyz.sh/
- Install Powerlevel10k : https://github.com/romkatv/powerlevel10k
- Use ~/.p10k.zsh and ~/.zshrc of this repo
- Launch :

```sh
git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://github.com/MichaelAquilina/zsh-you-should-use.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/you-should-use
git clone https://github.com/zdharma/fast-syntax-highlighting.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/fast-syntax-highlighting
```

## Node

Install latest LTS :

```sh
nvm install --lts
```

## Tilix config

Import the config with :

```sh
dconf load /com/gexperts/Tilix/ < tilix.dconf
```
