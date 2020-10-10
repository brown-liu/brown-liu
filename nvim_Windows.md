<h1>WINDOWS NEOVIM</h1>
1. download package ==>>  https://github.com/neovim/neovim/wiki/Installing-Neovim
2. install plugin =>>    remove-item alias:\curl and run $ curl -fLo ~/.config/nvim/autoload/plug.vim --create-dirs \ https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
3. make suer this folder is there C:\Users\LB87\AppData\Local\nvim\autoload and there is a plug.vim in it.
4
Plug 'roxma/nvim-completion-manager'
Plug 'SirVer/ultisnips'
Plug 'honza/vim-snippets'
Plug 'morhetz/gruvbox'
Plug 'bling/vim-airline'                                                                     
Plug 'vim-airline/vim-airline-themes'

set background =dark
colorscheme gruvbox

C++ syntax check
http://www.vim.org/scripts/script.php?script_id=4205
 " cppSyntaxCheck
let g:include_path=":../include:./include:./tinyxml"
let g:compile_flag="-D_LINUX_"
let g:cpp_compiler="/usr/bin/g++"
let g:enable_warning=1
let g:cpp_compiler="LANG=C g++ -Wall"


<h1>UBUNTU / MACOS NEOVIM</h1>
NVIM
Install the NeoVim AppimagePermalink Download and install the appimage, use the output-document option to rename it to nvim:
wget --quiet https://github.com/neovim/neovim/releases/download/nightly/nvim.appimage --output-document nvim Set the owner to root, and make nvim accessible to all users:

chmod +x nvim sudo chown root:root nvim Move the binary file to /usr/bin:

sudo mv nvim /usr/bin Move into your home directory and create the subfolder structure to store the configuration file:

cd ~ mkdir -p .config/nvim

sudo apt install curl

PLUGIN INSTALL
curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

python support
pip3 install --user neovim sudo apt-get install vim ln -s ~/.vim ~/.config/nvim ln -s ~/.vimrc ~/.config/nvim/init.vim

If autoload folder not exist, reinstall Plugin

@@@@@@ might need to CREATE ~/.vimrc.@@@@@

for file .vimrc

syntax on call plug#begin() Plug 'roxma/nvim-completion-manager' Plug 'SirVer/ultisnips' Plug 'honza/vim-snippets' Plug 'morhetz/gruvbox' call plug#end()

set background =dark colorscheme gruvbox
