# macOS Development Environment

This repository documents and configures my macOS development environment. It includes configurations for various tools and settings to enhance productivity and streamline the development workflow.

## Tools and Configurations

Here's a breakdown of the tools and configurations included in this repository:

- **Homebrew (brew):** Package manager for macOS. The `Brewfile` lists all the applications and tools installed via Homebrew.
- **Zsh:** The default shell. `zsh/zshrc` configures the Zsh environment, including aliases, functions, and environment variables.
- **Tmux:** Terminal multiplexer. `tmux/tmux.conf` configures the Tmux environment, including keybindings and plugin settings.
- **Neovim (nvim):** Text editor. `nvim/init.vim` and `nvim/vimrc` configure the Neovim environment, including plugins, color schemes, and keybindings.
- **VS Code (vscode):** Integrated Development Environment. `vscode/vscode.settings.json` configures VS Code settings, and `vscode/Default.code-profile` configures the default profile.
- **SketchyBar:** Status bar customization tool. `sketchybar/sketchybarrc` configures the SketchyBar, including widgets and their appearance.
- **Ghostty:** Terminal emulator. `ghostty/config` configures the Ghostty terminal emulator, and `ghostty/themes/` contains various themes.
- **mcp:** My custom command-line tool. `mcp/mcp.json` configures the tool, and `mcp/env` sets up the environment.
- **Aider:** AI pair programming tool. `aider/aider.yaml` configures aider.
- **Fonts:** Custom fonts for the terminal and editor. Includes the MesloLGS Nerd Font family.
- **Aerospace:** Window manager. `aerospace/aerospace.toml` configures the window manager.

## Installation and Setup

To set up this development environment, follow these steps:

1.  **Install Homebrew:**
    ```bash
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```
2.  **Install Brewfile dependencies:**
    ```bash
    brew bundle --file=./Brewfile
    ```
3.  **Configure Zsh:**
    -   Copy `zsh/zshrc` to `~/.zshrc`.
    -   Set Zsh as your default shell: `chsh -s $(which zsh)`
4.  **Configure Tmux:**
    -   Copy `tmux/tmux.conf` to `~/.tmux.conf`.
5.  **Configure Neovim:**
    -   Create the `~/.config/nvim` directory if it doesn't exist: `mkdir -p ~/.config/nvim`
    -   Copy `nvim/init.vim` to `~/.config/nvim/init.vim`.
    -   Copy `nvim/vimrc` to `~/.vimrc`.
6.  **Configure VS Code:**
    -   Copy `vscode/vscode.settings.json` to the VS Code settings directory.
    -   Copy `vscode/Default.code-profile` to the VS Code profile directory.
7.  **Configure SketchyBar:**
    -   Copy `sketchybar/sketchybarrc` to `~/.sketchybarrc`.
8.  **Configure Ghostty:**
    -   Copy `ghostty/config` to the Ghostty config directory.
    -   Copy themes from `ghostty/themes/` to the Ghostty themes directory.
9.  **Configure mcp:**
    -   Copy `mcp/mcp.json` to the appropriate location.
    -   Set up the environment variables as specified in `mcp/env`.
10. **Configure Aerospace:**
    -   Copy `aerospace/aerospace.toml` to the appropriate location.
11. **Install Fonts:**
    -   Install the fonts located in the `fonts/` directory.

## Usage

After completing the installation and setup, your macOS development environment should be configured and ready to use. You can customize the configurations further by modifying the respective configuration files.
```

I suggest you run these commands to copy the configuration files to the correct locations:

```bash
cp zsh/zshrc ~/.zshrc
cp tmux/tmux.conf ~/.tmux.conf
mkdir -p ~/.config/nvim
cp nvim/init.vim ~/.config/nvim/init.vim
cp nvim/vimrc ~/.vimrc
cp sketchybar/sketchybarrc ~/.sketchybarrc
cp ghostty/config ~/.config/ghostty/config.toml
cp aerospace/aerospace.toml ~/.aerospace.toml
```

Note: You'll need to manually install the fonts and configure VS Code settings and profile through the VS Code UI. Also, make sure to adjust the paths in `mcp/mcp.json` and `mcp/env` according to your system.
