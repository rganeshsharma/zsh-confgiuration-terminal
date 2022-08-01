# zsh-confgiuration-terminal
Follow the instructions for ZSH Terminal confguration on RHEL/CentOS/Fedora Systems:

1. ZSH install : sudo dnf install zsh -y

2. Change Shell from /bin/bash to /bin/zsh and Log out and Log in back and check if prompt has changed

3. Choose '0' for creating a empty zsh configuration file (~/.zshrc)

4. Download OhMyZSH Plugin Manager for configuring ZSH Plugins:
 sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

5. The main reason I recommend using ZSH is its Auto suggestions feature. 
   Download the OhMyZSH configuration and add the in plugins section in ~/.zshrc:

git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
 
plugins=( 
    # other plugins...
    zsh-autosuggestions
)

6.   Add ZSH Syntax Highlighter:
 git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
 
 plugins=( 
    # other plugins...
    zsh-autosuggestions
    zsh-syntax-highlighting
)

7.PowerLevel10K for prompt customizations:
  
