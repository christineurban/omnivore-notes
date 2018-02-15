# Vim
list current open vim sessions

    jobs

go to particular vim session

    fg %<job-id>   # from jobs
    
    # ex: fg %3

kill particular vim session

    kill %<job-id>

## Searching
search

    /<what-you-are-searching>

search and replace

    :%s/<thing-to-replace>/<replace-with>/gc   # global confirm

clear search

    /sdkfhlkdjf   # won't be able to find and will clear last search

## Shortcuts
save / quit / save and quit

    :w / :q / :wq

delete line / copy (yank) line

    dd / yy

delete to end of line

    d$ / y$

delete to beginning of line

    d^ / y^

put cursor at end of line

    A

sort

    :sort

expand fold

    # space bar

refold current fold

    za

refold all

    zm

see full path of current file

    # 1 then Ctrl+G



## Splits
split (open new file)

    :%sp

current directory

    %:h   # + tab to expand

jump between files

    [   # up
    ]   # down

maximize split

    +

minimize split

    -

equal size splits

    =