## Synopsis

This is Rohit's personal repository of scripts, settings and plugins for setting up a new system. This includes installing my settings for iterm2, zsh, vim, git, tmux as well as installing appropriate packages depending on if run on Ubuntu or macOS. Additionally we place some helper scripts in ~/bin/

## Motivation

This project exists because it is a pain to set up a new system every time you switch machines. This saves a days worth of work.

## Detailed List of Tools and customizations

+ vim plugins
..+ Vundle to allow installation of other plugins
..+ Syntastic for to lint code directly in vim
..+ ct..+p fuzzy finder for vim
..+ v..+airline for colorful status bar
..+ NERDTree for file browser capability
..+ supertab for better tab completion
+ Scripts in ~/bin/
..+ ss which rsync's your zsh, git to a machine you want to ssh into. e.g. ss 10.23.16.19
..+ my ..+ec2 which displays a list of ec2 instances and associated information in a nice table
..+ colourchart which shows you the color codes for theming in ..+..+zsh
..+ my du which does a du and sorts the results. e.g. my du /var/log/\*
..+ my ..+sqs which lists sqs queue
+ tmux configuration in tmux.conf
+ gitconfi..+ Please change this file if you use this repository
+ zs..+ Makes zsh the default shell and installs ..+..+zsh with my personal theme
+ Detect if Debian/Ubuntu/LinuxMint or MacOSX and Install packages
..+ Install PPAs and packages (See UbuntuPPA and UbuntuPackages file to see what is installed)
..+ Install relevant packages for MacOSX (Read Brewfile to see what is installed)
..+ MacOSX doesn't have a package for powerline fonts so install them manually
+ iterm2 configuration which can be loaded easily

## Installation

1. Review packages to be installed in Brewfile or UbuntuPackages to make sure you are ok with what will be installed.
2. Change .gitconfig to contain your specific email and username
3. Run ./install.sh
4. Open iterm2 and go to preferenc..+>gener..+">Load Preferences from a custom file or folder" and select the folder as ~/settings/iterm2_profile/

## Contributors

Rohit Pidaparthi and special thanks to Oleg Selivanov for ideas for the scripts in ~/bin/

## License

MIT
