# install terminal

MAC

xcode-select --install

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/Varut/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"


brew install zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"


git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
vi ~/.zshrc
ZSH_THEME="powerlevel10k/powerlevel10k"

source ~/.zshrc

git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

vi ~/.zshrc

plugins=(git docker docker-compose kubectl zsh-autosuggestions zsh-syntax-highlighting)


brew install fzf
brew install kubectx
brew install derailed/k9s/k9s

https://cloud.google.com/sdk/docs/install-sdk





Linux
sudo apt-get update
sudo apt-get install zsh -y
sudo chsh -s /usr/bin/zsh

git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
