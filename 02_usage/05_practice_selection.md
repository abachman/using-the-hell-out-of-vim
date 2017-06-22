!SLIDE normal
# Selection

Also known as "Visual Mode". Strong stuff.

    v V <C-v>

!SLIDE normal
# Selection

Works with simple movement

    vlllllll    " select seven characters to the right

!SLIDE normal
# Selection

Works with search

    vf=         " select everything on this line
                " up to and including the next =

    v/end<CR>   " select everything until you find
                " the next word 'end'

!SLIDE normal
# Yank and Paste

**y**ank, **p**aste, **c**hange, **d**elete

!SLIDE  normal
# Yank and Paste

    y p P
    c d
    yy dd

!SLIDE normal
# TEXT OBJECTS

**v**isual select **a**ll of a **w**ord, **c**hange **i**nside the **"**'s

!SLIDE normal
# TEXT OBJECTS

    vaw
    vi"
    va"
    ci(
    ciw

`text-objects`

!SLIDE normal
# TEXT OBJECTS

one command

    va"

!SLIDE normal
# TEXT OBJECTS

two parts

    va "

!SLIDE normal
# TEXT OBJECTS

verb - subject

    visual select all
    |
    va  "
        |
        of this quoted text

For example:

    They said, "you're crazy! |It'll never work!"
                              ^ cursor

    They said, "you're crazy! It'll never work!|"
               ----------------------------------
               ^ selection

!SLIDE normal
# TEXT OBJECTS

BLAM! `text-objects`!

    v[ia]_
         w  word
         s  sentence
         p  paragraph
         (  ()s
         [  []s
         {  {}s
         <  <>s
         t  html tag
         "  ""s
         '  ''s

!SLIDE normal
# It Goes Both Ways!

`o` while in visual mode puts the cursor at the **o**ther end of the selection.

!SLIDE normal
# **BONUS** TEXT OBJECTS

Also works with **c**hange, **d**elete, and **y**ank!

    c[ia]_
    d[ia]_
    y[ia]_
         w  word
         s  sentence
         p  paragraph
         (  ()s
         [  []s
         {  {}s
         <  <>s
         t  html tag
         "  ""s
         '  ''s

But visual first is nice because then you can see what you're doing.

!SLIDE
# Use a cheat sheet

!SLIDE center

![cheat sheet](vi-vim-cheat-sheet.gif)

!SLIDE normal bullets
# **s**ubstitutions

Command mode, finally!

One line:

    :s/this/that/

All lines:

    :%s/this/that/

Ask me each time:

    :%s/this/that/c
