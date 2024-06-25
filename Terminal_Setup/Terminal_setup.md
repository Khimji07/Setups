# Terminal Setup 

## First we need to update the system 
    sudo apt-get update

## After Updating the system, need to install zsh 
    sudo apt install zsh

## After installing the zsh, we need to change our current shell to zsh 
    chsh
        /bin/zsh

## Apply the shell change need to relogin the user.

## After login the user zsh ask to confiure it bur we can leave it by pressing "0" and we do the manual configuration with adding some extra tools like below.
    ohmyzsh
    zsh-autosuggestions
    zsh-syntax-highlighting
    powerlevel10k

## Now let's do the setup of oh-my-zsh tool.

### ogmyzsh Git Repository 
        https://github.com/ohmyzsh/ohmyzsh

    Install the git by below command
        apt install git

    Run command in terminal for install ohmyzsh
        Command sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

## Now let's do the setup of the zsh-autosuggestions.
    zsh-autosuggestions Git Repository
        https://github.com/zsh-users/zsh-autosuggestions

    Need to add zsh-autosuggestions in oh-my-zsh shell via cloning the repository.
        git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
    
    Add the plugin to the list of plugins for Oh My Zsh to load (inside ~/.zshrc):
        plugins=(git zsh-autosuggestions)

    After adding the plugin Start a new terminal session.

## Now let's do the setup of the zsh-syntax-highlighting.
    zsh-syntax-highlighting Git Repository
        https://github.com/zsh-users/zsh-syntax-highlighting

    Need to add zsh-syntax-highlighting in oh-my-zsh shell via cloning the repository..
        git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
    
    Activate the plugin in ~/.zshrc
        plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

    Restart zsh (such as by opening a new instance of your terminal emulator).

## Now let's do the setup of the powerlevel10k.
    powerlevel10k Git Repository
        https://github.com/romkatv/powerlevel10k

    Before adding powerlevel10k let's add additional font for extera beauty.
        sudo apt install -y fonts-font awesome

    Need to add powerlevel10k in oh-my-zsh shell via cloning the repository..
        git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k

    Set the below theme in ~/.zshrc.
        ZSH_THEME="powerlevel10k/powerlevel10k"

    After adding the theme restart the terminal

## After start the terminal they will ask for configuring powerlevel10k tools and then setup the tool configuration as you like.

## Enjoy. 