This is factor[e]'s recommended dotfile setup our developer team.  

Instructions
===

Clone the repo into ~/.factore-dotfiles 

    git clone https://github.com/factore/factore-dotfiles ~/.factore-dotfiles
    
**Linters**

Symlink all the linter dotfiles into your home folder

    for f in $(ls -d ~/.factore-dotfiles/linters/.*); do ln -s $f ~/; done && ls -al ~/
