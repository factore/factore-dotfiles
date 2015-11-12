This is factor[e]'s recommended dotfile setup our developer team.  

Instructions
===

Clone the repo into ~/.factore-dotfiles 

    git clone https://github.com/factore/factore-dotfiles ~/.factore-dotfiles
    
**Linters**

Symlink all the linter dotfiles into your home folder

    for f in $(ls -d ~/.factore-dotfiles/linters/.*); do ln -s $f ~/; done && ls -al ~/

Remember to just use these linters as a guideline, don't spend a ton of time trying to satisfy inane requirements (eg. you probably don't need top-level class documentation for your db/migrate classes, as much as Rubocop might want you to write one)

# Sublime

For Sublime users I've been using SublimeLinter (http://www.sublimelinter.com/en/latest/) and then the sub-packages for the individual linters (SublimeLinter-rubocop, SublimeLinter-contrib-eslint, SublimeLinter-contrib-scss-lint, SublimeLinter-coffeelint).  You also have to actually install the binaries that these linters rely on:

gem install rubocop (and rbenv rehash if you're an rbenv user)
gem install scss-lint (rbenv rehash)
npm install -g eslint
npm install -g coffeelint

