
# Git repository for managing dotfiles
Reference: https://www.ackama.com/what-we-think/the-best-way-to-store-your-dotfiles-a-bare-git-repository-explained/

Uses non-bare repository for managing documentation and README

Uses work-tree for keeping files in place instead of managing symlinks

## To clone:
git clone --bare <remote-git-repo-url> $HOME/.cfg
alias config='/usr/bin/git --git-dir=$HOME/.cfg/ --work-tree=$HOME'
config config --local status.showUntrackedFiles no
config checkout