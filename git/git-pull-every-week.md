# Git Pull Every Week

Backend Core (see [Alembic Issue](#alembic-issue) if issue)

             $ cd ../backend-core
             $ git co master
    (master) $ git pull
    (master) $ ./init.sh  # also runs ./migrate.sh
    
    # delete branches*

Panel

             $ cd ../panel
             $ git co master
    (master) $ git pull
    
    # delete branches*

API

             $ cd ../api
             $ git co master
    (master) $ git pull
    
    # go to tab 2 and restart API
    # delete branches*

Tasks

             $ cd ../tasks
             $ git co master
    (master) $ git pull
    
    # go to tab 3 and restart tasks
    # delete branches*

\*delete branches  

    (master) $ git br -vv   # list which branches are gone, verbose
    (master) $ git br -D branch-name   # delete branches marked done
    (master) $ git co branch-name
    (branch-name) $ git rebase master