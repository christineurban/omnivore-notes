# Git Pull Every Week

Backend Core (see [Alembic Issue](#alembic-issue) if issue)

             $ cd ../backend-core
             $ git co master
    (master) $ git pull
    (master) $ ./init.sh  # also runs ./migrate.sh
    
    # delete and rebase branches*

Panel

             $ cd ../panel
             $ git co master
    (master) $ git pull
    
    # delete and rebase branches*

API

             $ cd ../api
             $ git co master
    (master) $ git pull
    
    # go to tab 2 and restart API
    # delete and rebase branches*

Tasks

             $ cd ../tasks
             $ git co master
    (master) $ git pull
    
    # go to tab 3 and restart tasks
    # delete and rebase branches*

Marketplace UI

             $ cd ../marketplace-ui
             $ git co master
    (master) $ git pull
    
    # delete and rebase branches*

Marketplace API

             $ cd ../marketplace-api
             $ git co master
    (master) $ git pull
    
    # delete and rebase branches*

\*delete branches  

    (master) $ git br -vv   # list which branches are gone, verbose
    (master) $ git br -D branch-name   # delete branches marked done

\*rebase branches

    (master) $ git co branch-name
    (branch-name) $ git st    
    (branch-name) $ git stash # if any changes
    (branch-name) $ git rebase master
    (branch-name) $ git st   # if diverged do git push -f
    (branch-name) $ git stash pop   # if changes were stashed