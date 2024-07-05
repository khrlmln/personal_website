# Download and Install Firefox

```bash
curl -O https://download-installer.cdn.mozilla.net/pub/firefox/releases/127.0.2/linux-x86_64/en-US/firefox-127.0.2.tar.bz2
```

```bash
tar xjf firefox-\*.tar.bz2
```

```bash
sudo mv firefox /opt
```

```bash
sudo ln -s /opt/firefox/firefox /usr/bin/firefox
```

```bash
curl -O https://raw.githubusercontent.com/mozilla/sumo-kb/main/install-firefox-linux/firefox.desktop -P /usr/share/applications
```

# Download Google Chrome Stable

```bash
curl -O https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
```

# GitHub CLI

```bash
type -p curl >/dev/null || (sudo apt update && sudo apt install curl -y)
curl -fsSL https://cli.github.com/packages/githubcli-archive-keyring.gpg | sudo dd of=/usr/share/keyrings/githubcli-archive-keyring.gpg \
&& sudo chmod go+r /usr/share/keyrings/githubcli-archive-keyring.gpg \
&& echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/githubcli-archive-keyring.gpg] https://cli.github.com/packages stable main" | sudo tee /etc/apt/sources.list.d/github-cli.list > /dev/null \
&& sudo apt update \
&& sudo apt install gh -y
```

# VS Code

```bash
https://vscode.download.prss.microsoft.com/dbazure/download/stable/ea1445cc7016315d0f5728f8e8b12a45dc0a7286/code_1.91.0-1719861592_amd64.deb
```

# Starship

```bash
curl -sS https://starship.rs/install.sh | sh
```

# Fira Nerd Fonts

```bash
https://github.com/ryanoasis/nerd-fonts/releases/download/v3.2.1/FiraCode.zip
```

```bash
https://github.com/ryanoasis/nerd-fonts/releases/download/v3.2.1/FiraMono.zip
```

# Cascadia Code Font

```bash
https://github.com/microsoft/cascadia-code/releases/download/v2404.23/CascadiaCode-2404.23.zip
```

# VS Code Settings.json

```bash
https://gist.githubusercontent.com/khrlmln/1cd7b24ae9f07c57c1b7bc07a81e6b2e/raw/99d6580ea293b3d871230895b52c73790800f1ad/settings.json
```

# Starship.toml config file

```bash
https://gist.githubusercontent.com/khrlmln/8165ede109a2cac7b1d3f384dd06dbab/raw/af376dbed89578b2f0122d60deced08bca655818/starship.toml
```

# Change shell to zsh

> Install following packages for ZSH Shell

```bash
sudo apt install zsh-autosuggestions zsh-common zsh-syntax-highlighting zsh
```

> Change Default Shell

    ```bash
    chsh
    ```

> Type password and use /bin/zsh as default shell.

# .zshrc file

```bash
https://gist.githubusercontent.com/khrlmln/ee80025b00720d9dd6ba2f4c8ab96131/raw/0534b3101259f1565731084530478d1299859623/.zshrc
```

# Setup Sudo No Password in Linux Terminal

> Open the terminal and type the following command to get /etc/sudoers file:

```bash
sudo visudo
```

> Enter the credential to get the file:

> Scroll down till the end of the /etc/sudoers file and append the mentioned below line:

```bash
mln-khrl ALL=(ALL) NOPASSWD:ALL
```

> Press Ctrl+s to save the /etc/sudoers file and then Ctrl+x to exit it.

# List total number of installed packages

```bash
dpkg -l | wc -l
```

```bash
dpkg --get-selections | grep -w "install" | wc -l
```
