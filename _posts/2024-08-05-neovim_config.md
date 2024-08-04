---
layout: post
title: "My Neovim Config"
date: 2024-08-04 00:00:00 +0000
categories: Linux
tags: [neovim,config]
---

### [Link to my config](https://github.com/DK10WS/Neovim/)

# Why Neovim

I have tried all the best IDEs out there, from VSCode to Notepad, but they were either very cluttered or lacked features that I really needed. Then I stumbled onto [Vim](https://www.vim.org/) , which did not scream IDE to me. However, a friend showed me how Vim works and what the Vim workflow is like. I was really intrigued by how a text editor could be so complex.

I researched more, got to know about [Neovim](https://neovim.io/) and its plugin architecture, and started with [NvChad](https://nvchad.com/). At first, I did not quite understand how NvChad worked, but the more I used it, the more I understood it, and my life got more easier with Neovim. Then, I wanted LSP in Neovim but never understood how to integrate it into NvChad, so I decided to write my own [config](https://github.com/DK10WS/Neovim/) for Neovim to understand how these plugins actually work.

# How to start writing your own config

> This is not a Guide on how to write your own config rather what is required to write your config

You can use any tutorial you like, or you can set it up yourself by reading the documentation and understanding how each plugin actually functions and how you can modify its behavior. **Its not necessary to know lua to write your own config but its better if you know**.

If you choose to write it yourself, then

1. The first thing you need is a plugin manager I choose [Lazy](https://github.com/folke/lazy.nvim) as it has a great GUI, fast and quite easy to use, there are many other like [packer](https://github.com/wbthomason/packer.nvim) and [paq](https://github.com/savq/paq-nvim)

2. Once you have a package manager you need a manager for LSP servers, DAP servers, linters, and formatters. [Mason](https://github.com/williamboman/mason.nvim) is the best out there for this job

3. Now that you have all required package managers you can start with adding your first plugin

4. First plugin i got was [tree-sitter](https://github.com/tree-sitter/tree-sitter) to highlight my keywords and make the code have different color based on

5. Then next was [telescope](https://github.com/nvim-telescope/telescope.nvim) which is great to find, jump between your work in a project directory.

6. Then comes the most important part the [lsp](https://github.com/neovim/nvim-lspconfig) which has to installed using mason. This is the most confusing part of the config if you get stuck or do not understand how to configure check out this [video](https://www.youtube.com/playlist?list=PLsz00TDipIffreIaUNk64KxTIkQaGguqn) for clear explanation on lsp configuration

7. Major Work of your configuration is done now you can add [none-ls](https://github.com/nvimtools/none-ls.nvim), This is used to indent and format your code properlike like prettier in Vscode.

8. These many plugins should get you started you can also reffer to my [config](https://github.com/DK10WS/Neovim/) to see more uselful plugins i have installed.

The main Purpose of writing your own config is to identify what you need and search it up and you will find a plugin for it, You can also ask on [neovim reddit](https://www.reddit.com/r/neovim/) if you get stuck at any point.
