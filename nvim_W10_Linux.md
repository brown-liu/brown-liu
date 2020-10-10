<h1>WINDOWS NEOVIM</h1>
1. download package ==>>  https://github.com/neovim/neovim/wiki/Installing-Neovim
<br>2. install plugin =>>    remove-item alias:\curl and run $ curl -fLo ~/.config/nvim/autoload/plug.vim --create-dirs \ https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
<br>3. make suer this folder is there C:\Users\LB87\AppData\Local\nvim\autoload and there is a plug.vim in it.
<br>4
Plug 'roxma/nvim-completion-manager'
<br>Plug 'SirVer/ultisnips'
<br>Plug 'honza/vim-snippets'
<br>Plug 'morhetz/gruvbox'
<br>Plug 'bling/vim-airline'                                                                     
<br>Plug 'vim-airline/vim-airline-themes'

<br>set background =dark
<br>colorscheme gruvbox

<br>C++ syntax check
<br>http://www.vim.org/scripts/script.php?script_id=4205
<br> " cppSyntaxCheck
<br>let g:include_path=":../include:./include:./tinyxml"
<br>let g:compile_flag="-D_LINUX_"
<br>let g:cpp_compiler="/usr/bin/g++"
<br>let g:enable_warning=1
<br>let g:cpp_compiler="LANG=C g++ -Wall"


<h1>UBUNTU / MACOS NEOVIM</h1>
<br>NVIM
<br>Install the NeoVim AppimagePermalink Download and install the appimage, use the output-document option to rename it to nvim:
<br>wget --quiet https://github.com/neovim/neovim/releases/download/nightly/nvim.appimage --output-document nvim Set the owner to root, and make nvim accessible to all users:

<br>chmod +x nvim sudo chown root:root nvim Move the binary file to /usr/bin:

<br>sudo mv nvim /usr/bin Move into your home directory and create the subfolder structure to store the configuration file:

<br>cd ~ mkdir -p .config/nvim

sudo apt install curl

<br>PLUGIN INSTALL
<br>curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

<br>python support
<br>pip3 install --user neovim sudo apt-get install vim ln -s ~/.vim ~/.config/nvim ln -s ~/.vimrc ~/.config/nvim/init.vim

<br>If autoload folder not exist, reinstall Plugin

<br>@@@@@@ might need to CREATE ~/.vimrc.@@@@@

<br>for file .vimrc

<br>syntax on call plug#begin() Plug 'roxma/nvim-completion-manager' Plug 'SirVer/ultisnips' Plug 'honza/vim-snippets' Plug 'morhetz/gruvbox' call plug#end()

<br>set background =dark colorscheme gruvbox
