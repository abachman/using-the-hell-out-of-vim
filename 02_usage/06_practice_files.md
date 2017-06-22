!SLIDE normal bullets
# Handling Multiple Files

* Splitting windows
* Working between files (hint: unix-style rears it's head)

!SLIDE normal bullets
# Splitting windows

&lt;C-w&gt; + ...

* **v**ertical split
* horizontal **s**plit
* **q**uit

!SLIDE normal

# Moving around splits

Shortcuts (highly recommended)

    inoremap <C-h> <esc><C-w><C-h>
    inoremap <C-j> <esc><C-w><C-j>
    inoremap <C-k> <esc><C-w><C-k>
    inoremap <C-l> <esc><C-w><C-l>
    noremap <C-h> <C-w><C-h>
    noremap <C-j> <C-w><C-j>
    noremap <C-k> <C-w><C-k>
    noremap <C-l> <C-w><C-l>

!SLIDE normal
# Helpful Plugins for Multi-file Work

## ag / ack

Search - `ag` https://github.com/ggreer/the_silver_searcher

Vim integration - `ack.vim` https://github.com/mileszs/ack.vim

## NERDTree

File browser - https://github.com/scrooloose/nerdtree

## ctrlp

Fuzzy file finder - https://github.com/kien/ctrlp.vim
