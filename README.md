<div align="center">
  <h1>My Neovim setup</h1>
  <p align="center">
    <img src="https://img.shields.io/badge/Lua-2C2D72?style=for-the-badge&logo=lua&logoColor=white"/>
    <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black"/>
  </p>
  <p>
    <img src="https://img.shields.io/badge/Maintained%3F-yes-green.svg"/>
  </p>
  <p>
    <img src="https://raw.githubusercontent.com/bjchavez/nvim/main/docs/imgs/preview01.png"/>
    <img src="https://raw.githubusercontent.com/bjchavez/nvim/main/docs/imgs/preview02.png"/>
  </p>
</div>

## Current updates

- **Current theme:** [Tokyonight-storm](https://github.com/folke/tokyonight.nvim)
- **Current font:** [UbuntuMono Nerd Font](https://www.programmingfonts.org/#ubuntu)

## Requirements

- [Neovim](https://neovim.io/) >= 0.8.0
- Install a font from [nerdfonts.com](https://www.nerdfonts.com/)

## Installation

- ### Clone this repository
```
git clone https://github.com/bjchavez/nvim.git ~/.config/nvim
```
- ### Delete preview and .git folders
```
sudo rm -rf ~/.config/nvim/preview
sudo rm -rf ~/.config/nvim/.git
```
- ### Run
```
nvim
```

## Plugins list

- [telescope](https://github.com/nvim-telescope/telescope.nvim)
- [treesitter](https://github.com/nvim-treesitter/nvim-treesitter)
- [lsp-zero](https://github.com/VonHeikemen/lsp-zero.nvim)
- [lualine](https://github.com/nvim-lualine/lualine.nvim)
- [mini](https://github.com/echasnovski/mini.nvim)
- [nvterm](https://github.com/NvChad/nvterm)
- [autopairs](https://github.com/windwp/nvim-autopairs)
- [gitsigns](https://github.com/lewis6991/gitsigns.nvim)
- [markdown-preview](https://github.com/iamcco/markdown-preview.nvim)
- [indent-blankline](https://github.com/lukas-reineke/indent-blankline.nvim)
- [web-devicons](https://github.com/nvim-tree/nvim-web-devicons)
- [styler](https://github.com/folke/styler.nvim)
- [telescope-file-browser](https://github.com/nvim-telescope/telescope-file-browser.nvim)

## Main folders
```
├── lua
│   ├── core
│   └── plugins
│       ├── configs
│       └── utils
└── ...
```

## Plugins structure

```
├── plugins
│   ├── telescope.lua
│   ├── treesitter.lua
│   ├── lsp.lua
│   ├── lualine.lua
│   ├── mini.lua
│   ├── nvtem.lua
│   ├── autopairs.lua
│   ├── colorscheme.lua
│   │   ├── tokyonight.nvim
│   │   └── catppuccin/nvim
│   ├── gitsigns.lua
│   ├── markdown-preview.lua
│   ├── indent.lua
│   ├── web-devicons.lua
│   ├── styles.lua
│   ├── telescope-file-browser.lua
│   └── lsp.lua
└── ...
```

## Keymaps

> **IMPORTANT**: the `space-bar` remains as the `<leader>` key.

**`SOME VIM MODES USED`**: **`[N]ORMAL`** - **`[V]ISUAL`** - **`[I]NSERT`** - **`[T]ERMINAL`**

### General

| Mode      | Keymap           | Description                          |
| :----:    | :----:           | ----------------------------------   |
| N - I - V | `Ctrl` + `s`     | Save file                            |
| N         | `Ctrl` + `q`     | Quit                                 |
| N         | `Ctrl` + `x`     | Quit and throw away unsave changes   |
| N         | `Ctrl` + `h`     | Go to left window                    |
| N         | `Ctrl` + `j`     | Go to lower window                   |
| N         | `Ctrl` + `k`     | Go to upper window                   |
| N         | `Ctrl` + `l`     | Go to right window                   |
| N         | `leader` + `v`   | Vertical split                       |
| N         | `leader` + `h`   | Horizontal split                     |
| N         | `leader` + `bd`  | Delete current buffer                |
| N         | `Ctrl` + `Up`    | Increase window height               |
| N         | `Ctrl` + `Down`  | Decrease window height               |
| N         | `Ctrl` + `Left`  | Increase window width                |
| N         | `Ctrl` + `Right` | Decrease window width                |

### Telescope

| Mode      | Keymap           | Description                          |
| :----:    | :-----:          | ----------------------------------   |
| N         | `leader` + `ff`  | Find files                           |
| N         | `leader` + `bf`  | Show buffers                         |
| N         | `leader` + `gs`  | Show git status                      |
| N         | `leader` + `gc`  | Show git commits                     |
| N         | `leader` + `t`   | Telescope                            |

### Telescope File Browser

| Mode      | Keymap           | Description                          |
| :----:    | :-----:          | ----------------------------------   |
| N         | `c`              | Create file / folder                 |
| N         | `r`              | Rename file / folder                 |
| N         | `m`              | Move file / folder                   |
| N         | `y`              | Copy file / folder                   |
| N         | `d`              | Delete file / folder                 |
| N         | `o`              | Open file / browser                  |
| N         | `g`              | Go to parent dir                     |
| N         | `e`              | Go to home dir                       |
| N         | `w`              | Go to current working dir            |
| N         | `t`              | Change current workking dir          |
| N         | `s`              | Toggle all                           |

### Nvterm

| Mode      | Keymaps          | Description                          |
| :----:    | :------:         | ----------------------------------   |
| N         | `Alt` + `i`      | Show terminal                        |
| T         | `Alt` + `t`      | Hide terminal                        |

### Markdown Preview

| Mode      | Keymaps          | Description                          |
| :----:    | :------:         | ----------------------------------   |
| N         | `leader` + `mp`  | Show markdown preview window         |
| N         | `leader` + `ms`  | Close markdown preview window        |

### LSP

| Mode      | Keymaps          | Description                          |
| :----:    | :------:         | ----------------------------------   |
| N         | `gd`             | Go to definition                     |
| N         | `gh`             | Show float definition                |
| N         | `leader` + `n`   | Go to next diagnostic                |
| N         | `leader` + `m`   | Go to previous diagnostic            |

## FAQ

- **Why does my configuration look different?**

  I update my neovim configuration daily. I change the themes and keymaps, but I will do my best to write a good documentation.

- **Can I copy code for personal use?**

  Yes of course. That's the goal. Luck 😉

## License

[MIT License](LICENSE)
