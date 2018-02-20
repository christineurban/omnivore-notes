# Git Pull Every Week

Backend Core (see [Alembic Issue](#alembic-issue) if issue)

    (master) $ ../backend-core
    (master) $ ./init.sh  # also runs ./migrate.sh
    
    # delete branches*

Panel

    (master) $ ../panel
    
    # delete branches*

API

    (master) $ ../api
    
    # go to tab 2 and restart API
    # delete branches*

Tasks

    (master) $ ../tasks
    
    # go to tab 3 and restart tasks
    # delete branches*

\*delete branches  

    (master) $ git br -vv   # list which branches are gone, verbose
    (master) $ git br -D branch-name   # delete branches marked done
    (master) $ git co branch-name
    (branch-name) $ git rebase master