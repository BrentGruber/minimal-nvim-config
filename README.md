# minimal-nvim-config

A very small Neovim configuration built around a single `init.lua`.

This setup keeps the moving parts intentionally limited while still covering the basics for day to day editing:

- line numbers and relative numbers
- simple leader key mappings
- a minimal plugin set using `vim.pack`
- file navigation with `oil.nvim`
- fuzzy picking with `mini.pick`
- built-in LSP setup for several common languages
- formatting through Neovim's LSP client
- `vague.nvim` for colors

## Philosophy

The goal of this config is to stay lightweight and readable.

Instead of a large framework or many layers of abstraction, everything lives in one file so it is easy to inspect, modify, and understand.

## Included plugins

- [`vague.nvim`](https://github.com/vague2k/vague.nvim) for colors
- [`oil.nvim`](https://github.com/stevearc/oil.nvim) for file browsing
- [`mini.pick`](https://github.com/echasnovski/mini.pick) for picker functionality
- [`nvim-lspconfig`](https://github.com/neovim/nvim-lspconfig) for language server configuration
- [`typst-preview.nvim`](https://github.com/chomosuke/typst-preview.nvim) for Typst preview support

## Key mappings

- `<leader>o` reload and source the current config
- `<leader>w` write file
- `<leader>q` quit
- `<leader>f` open file picker
- `<leader>h` open help picker
- `<leader>lf` format with LSP

Leader is set to space.

## LSP servers enabled

This config enables the following servers/tools through Neovim's LSP support:

- `lua_ls`
- `svelte-language-server`
- `pyright`
- `gopls`
- `zls`
- `alejandra`
- `bash-language-server`
- `marksman`
- `yaml-language-server`
- `vscode-langservers-extracted`

You will need those language servers installed separately on your system for them to work.

## Requirements

- Neovim with support for `vim.pack`
- the language servers you want to use installed separately

## Layout

```text
.
├── init.lua
└── README.md
```

## Why this repo exists

This repo is a clean starting point for a personal Neovim setup that does not depend on a large distro, plugin manager framework, or heavy folder structure.

It is best suited for someone who wants:

- a small config
- fast startup into a usable editor
- a setup that is easy to learn from and customize
