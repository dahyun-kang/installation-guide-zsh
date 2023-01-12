# Development environment installation guidelines

[cuda](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html), [zsh](https://github.com/ohmyzsh/ohmyzsh), [anaconda](https://www.anaconda.com/), [dotfiles](https://github.com/wookayin/dotfiles) on Ubuntu

## Prerequisites
* Ubuntu >= 16.04
* Download [Anaconda installer](https://www.anaconda.com/products/individual)

## root >>
Install cuda manually following [NVIDIA CUDA Installation Guide for Linux](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html), and then


    sudo apt-cache search nvidia-driver
    sudo apt-get install nvidia-driver-4**
    sudo apt-get install cuda
    sudo apt-get nvidia-cuda-toolkit
    sudo reboot
    
    sudo apt-get install curl
    sudo apt-get install zsh

## user >>
    chsh -s $(which zsh)
    sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
    bash Anaconda3_LATEST.sh
    curl -fsSL https://dotfiles.wook.kr/etc/install | bash
    source /home/USERNAME/anaconda3/bin/activate
    conda init zsh
    dotfile update
    source ~/.dotfiles/zsh/zshrc

## user (at local macbook) >>
    git clone https://github.com/powerline/fonts.git
    cd fonts
    ./install.sh
    
 Open `ITerm2 > Preferences > Profiles > Text > Change Font` and set it to something that has “for Powerline”.
 Some contents were adapted from [here](https://www.freecodecamp.org/news/jazz-up-your-zsh-terminal-in-seven-steps-a-visual-guide-e81a8fd59a38/)
