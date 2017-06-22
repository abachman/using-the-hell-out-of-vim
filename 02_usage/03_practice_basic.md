!SLIDE normal
# Basic Skills

Open, close, edit, save.

!SLIDE code
# Basic Skills

    @@@vim
    vim, i, <esc>, :q, :e, :w, <CR>

!SLIDE normal bullets incremental
## Modal Editing

* **Normal** - movement and action
* **Visual** - selection
* **Insert** - boring old plain old typing
* **Command** - substitution and plugin commands
* **Ex-mode** - only by accident
* **Search?** - it's kind of like a mode?

!SLIDE normal bullets incremental

# *Digression*

## vimrc

* this is where your customizations will go. yours will be unique to you.
* but for your sanity, make saving easier
* and make things prettier

!SLIDE code
# *Digression*

    @@@vim

    " saving
    map <D-s> :w<CR>           " just save
    imap <D-s> <esc>:w<CR>     " save and return to normal mode
    vmap <D-s> <esc>:w<CR>gv   " save and reselect

    " colors
    syntax on                  " Enable syntax highlighting
    filetype plugin indent on  " Enable filetype-specific
                               " indenting and plugins
    set background=dark        "
    colorscheme desert         " best non-Solarized scheme

