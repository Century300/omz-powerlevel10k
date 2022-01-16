# Install oh-my-zsh, custom .zshrc, powerlevel10k theme
These are 2 bash scripts to fast install some packages to a host machine.

I used these scripts to install oh-my-zsh, my .zshrc configuration, and powerlevel10k theme to the Ubuntu & Kali (Linux) machines on TryHackMe.com, I have not tested the scripts with other machines yet.

### My .zshrc configuration
- Theme: powerlevel10k/powerlevel10k (including the official supported fonts [MesloLGS](https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k)).
- Plugins used from $HOME/.oh-my-zsh/plugins/: git sudo web-search dirhistory history jsontools colored-man-pages command-not-found autojump
- Added custom plugins in $HOME/.oh-my-zsh/custom/plugins/: zsh-autosuggestions k zsh-syntax-highlighting

## Instructions
- Clone the repo to _~/Downloads/omz-powerlevel10k_ to install Meslo Fonts properly
```bash
git clone https://github.com/Century300/omz-powerlevel10k.git ~/Downloads/omz-powerlevel10k && cd ~/Downloads/omz-powerlevel10k && sudo chmod +x install*
```
- Intall part 1, type "Y" when you see "_Do you want to change your default shell to zsh?_"
```
./install_zsh_part1.sh
```
- Install part 2
```bash
./install_zsh_part2.sh
```
- Source the .zshrc file and remove the cloned repo
```bash
source ~/.zshrc
sudo rm -rf ~/Downloads/omz-powerlevel10k
```
