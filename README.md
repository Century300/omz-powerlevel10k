# Install oh-my-zsh, custom .zshrc, powerlevel10k theme
These are 2 bash scripts to fast install some packages to a host machine.

I used these scripts to install oh-my-zsh, my .zshrc configuration, and powerlevel10k theme to the Ubuntu & Kali (Linux) machines on TryHackMe.com, I have not tested the scripts with other machines yet.

### My .zshrc configuration
- Theme: powerlevel10k/powerlevel10k (including the official supported fonts [MesloLGS](https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k)).
- Plugins used from $HOME/.oh-my-zsh/plugins/: git sudo web-search dirhistory history jsontools colored-man-pages command-not-found autojump
- Added custom plugins in $HOME/.oh-my-zsh/custom/plugins/: zsh-autosuggestions k zsh-syntax-highlighting

## Instructions
- git clone https://github.com/Century300/omz-powerlevel10k.git ~/Downloads/omz-powerlevel10k (require this path to install Meslo Fonts properly)
- cd ~/Downloads/omz-powerlevel10k
- sudo chmod +x install*
- ./install_zsh_part1.sh
- _(type Y when you see "Do you want to change your default shell to zsh?")_
- ./install_zsh_part2.sh
- source ~/.zshrc
- sudo rm -rf ~/Downloads/omz-powerlevel10k
