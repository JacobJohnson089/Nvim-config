# Nvim-config

```
:set number
:set autoindent
:set tabstop=4
:set shiftwidth=4
:set smarttab
:set softtabstop=4
:set mouse=a

call plug#begin()

Plug 'https://github.com/vim-airline/vim-airline' " Status bar
Plug 'https://github.com/preservim/nerdtree' " NerdTree
Plug 'http://github.com/tpope/vim-surround' " Surrounding ysw)
Plug 'https://github.com/tpope/vim-commentary' " gcc & gc for commenting
Plug 'https://github.com/ap/vim-css-color'
Plug 'https://github.com/rafi/awesome-vim-colorschemes'
Plug 'https://github.com/ryanoasis/vim-devicons' " dev icons
Plug 'https://github.com/tc50cal/vim-terminal'
Plug 'https://github.com/preservim/tagbar' " Tagbar for code navigation

call plug#end()

nnoremap <C-t> :NERDTreeFocus<CR>
nnoremap <C-f> :NERDTreeToggle<CR>
nnoremap <C-t> :NERDTreeRefreshRoot <CR>
nnoremap <C-b> :TagbarToggle<CR>
nnoremap <C-p> :TerminalSplit bash<CR>`
inoremap <expr> <Tab> pumvisible() ? coc#_select_confirm() : "<Tab>"
nmap <F8>:TagbarToggle<CR>
```

# Requirements
-Plug
[Installing Plug](https://github.com/junegunn/vim-plug)

# Installation
Linux
```
sudo apt install neovim
```
Arch Linux
```
su
pacman -S neovim
```
go in the ```home/usr``` Directory 
```
mkdir .config
cd .config
mkdir nvim
cd nvim
nvim init.vim
```
# Installing the Plugins
Paste into init.vim (Ctrl-Shift-V)
execute ```:PlugInstall``` into the vim command to install all the plugins 
execute ```:wq``` to quit save
