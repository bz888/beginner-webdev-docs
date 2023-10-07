### Setup (macos)

- Prequistie
  - Terminal choice:
  - Currently I am using iterm2, which you can install using `brew install --cask iterm2` assuming brew doctor is installed,else you can download from their website `https://iterm2.com/downloads.html`

1. Start the terminal and make `zsh` the default shell
   - Run `zsh --version` in your terminal to determine if you already have `zsh` installed
     - If you do:
       - Run `chsh -s $(which zsh)`
       - Restart the terminal (or log out and back into your computer)
       - Move on to step 2
     - If not, you'll need to install it by following the OS specific instructions below:
       - Linux
         - `sudo apt-get install zsh`
         - `chsh -s $(which zsh)`
         - Restart the terminal (or log out and log back in to your computer)
       - MacOS
         - Install [Homebrew](https://brew.sh/) with `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
         - Verify it is setup correctly with `brew doctor`
         - You will be requested to install the Command Line Developer Tools from Apple. Confirm by clicking Install. After the installation finished, continue installing Homebrew by hitting Return again.
         - Install zsh with `brew install zsh`
         - Make it the default shell: `sudo sh -c "echo $(which zsh) >> /etc/shells" && chsh -s $(which zsh)`
         - Restart the terminal (or log out and log back in to your computer)
1. Open a terminal and if you are prompted to make a choice, choose `q`.
1. Install oh-my-zsh from inside the terminal
   - `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
   - Restart the terminal
1. Install VS Code if it isn't already installed
1. In your terminal, open VS Code with `code .`
1. Install the following VS Code extensions
   - ESLint
   - Live Share (online students only)
   - vscode-icons (optional, but pretty :wink:)
   - GitLens (optional)
1. Install nvm
   - `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash`
1. Move the 3 nvm lines from the bottom of `~/.bash_profile` (or if they aren't there, check out `~/.bashrc`) to the bottom of `~/.zshrc`
1. Change the oh-my-zsh theme at the top of the `.zshrc` file from `bobbyrussell` to `bira`
1. Close and reopen your terminal
   - If your command prompt now looks different (e.g. showing your computer name) that's a good sign
1. `nvm install --lts`

### Docker

#### notes: Docker is very useful

1. Install
   - Just install from the website, and should be good to go (`https://docs.docker.com/desktop/install/mac-install/`)

### Optional

#### notes: I currently don't use VS code as my default editor, if you have more perfered alternatives you can skip this step

1. Make VS Code your default Git editor
   - Run this command in your terminal: `git config --global core.editor "code --wait"`
1. Enable automatic colour-coding of brackets and automatic fixing of linting errors on file save
   - In VS Code, click the Settings cog button in the bottom left and open the Command Palette. Type `settings.json` into the little search box that appears at the top of your screen, and then click on the `Preferences: Open Settings (JSON)` option to open your `settings.json` config file. Paste in these contents:
   ```json
   "editor.bracketPairColorization.enabled": true,
   "editor.codeActionsOnSave": { "source.fixAll.esLint": true }
   ```
   - Note that each entry in your `settings.json` should end in a comma except for the last one, so if there are some existing entries you'll need to add a comma before pasting the above lines1. Sta
