# .files

When I update my laptop to Yosemite, I created this to help set my computer up a little faster.

## Installation

    cd ~
    git init
    git remote add origin https://github.com/wtsnz/dotfiles.git
    git pull origin master

Thanks to [Sam Soffes](https://github.com/soffes/dotfiles/blob/master/Readme.markdown) I can hide files that I don't want to see in my home directory like so

    SetFile -a "V" ~/README.md ~/Brewfile

### Xcode

Install Xcode using the App Store app.

### Hombrew

[Install Homebrew](http://brew.sh) along with my default apps:

    ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    brew doctor
    cd ~
    brew bundle

### Install oh-my-zsh

    curl -L https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh | sh

### Ruby 2.1.3

Install Ruby, and set it as the global version

    rbenv install 2.1.3
    rbenv global 2.1.3

## OSX Preferences

Open a terminal and run the commands

    #Set a blazingly fast keyboard repeat rate
    defaults write NSGlobalDomain KeyRepeat -int 0.02

    # Show hidden files
    defaults write com.apple.finder AppleShowAllFiles -boolean true ; killall Finder

    #Show the ~/Library folder
    chflags nohidden ~/Library

    #Store screenshots in subfolder on desktop
    mkdir ~/Desktop/Screenshots
    defaults write com.apple.screencapture location ~/Desktop/Screenshots

## Apps to install from the App Store
A few apps that I can't live without

- Tweetbot
- Logic Pro X
- Keynote
- Sketch
