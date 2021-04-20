# Development environment installation guidelines
#### zsh, anaconda, dotfiles

## Prerequisites
* Ubuntu >= 16.04
* Download [Anaconda installer](https://www.anaconda.com/products/individual)

## root >>

    sudo apt-get install curl
    sudo apt-get install zsh

## user >>
    chsh -s $(which zsh)                      
    bash Anaconda3_LATEST.sh
    curl -fsSL https://dotfiles.wook.kr/etc/install | bash
    source /home/USERNAME/anaconda3/bin/activate
    conda init zsh
    dotfile update

## References
[Anaconda](https://www.anaconda.com/)

[Oh-My-Zsh](https://github.com/ohmyzsh/ohmyzsh)

[dotfiles](https://github.com/wookayin/dotfiles)
