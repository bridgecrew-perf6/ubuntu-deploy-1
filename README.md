# ubuntu-deploy

Update packages
```sh
sudo apt update && sudo apt upgrade -y
```

Install additional packages
```sh
sudo apt install -y zsh neovim unzip network-manager rtl8821ce-dkms exa fd-find
```

Install oh-my-zsh
```sh
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Download `.zshrc`
```sh
wget https://raw.githubusercontent.com/billykirk01/ubuntu-deploy/main/.zshrc
```

Install Rust
```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Install Deno
```sh
curl -fsSL https://deno.land/install.sh | sh
```

Install Go
```sh
wget "https://go.dev/dl/$(curl https://go.dev/VERSION\?m\=text).linux-amd64.tar.gz"
sudo rm -rf /usr/local/go && sudo tar -C /usr/local -xzf go*linux-amd64.tar.gz
```

Install vim-plug
```
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```

Download `.vimrc`
```sh
wget https://raw.githubusercontent.com/billykirk01/ubuntu-deploy/main/.vimrc
```
