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
