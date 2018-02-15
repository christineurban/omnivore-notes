# Git Pull Every Week

Backend Core
- `(master) $ ../dev/backend-core`
- `(master) $ ./init.sh` (also runs ./migrate.sh) 
- (see [Alembic Issue](##alambic-issue) if issue)
- delete branches*

Panel
- `(master) $ ../dev/panel`
- delete branches*

API
- `(master) $ ../dev/api`
- go to tab 2 and restart API
- delete branches*

Tasks
- `(master) $ ../dev/tasks`
- go to tab 3 and restart tasks
- delete branches*

\*delete branches  
 - `(master) $ git br -vv` (list which branches are gone, verbose) 
 - `(master) $ git br -D` (delete branches marked done) 
 - `(master) $ git co branch-name`
 - `(branch-name) $ git rebase master`


## Alembic Issue (Backend Core)

`(branch-name) $ alembic downgrade -1`

`(branch-name) $ git co master`

`(master) $ ./migrate.sh`

`(master) $ git co branch-name`

`(branch-name) $ git rebase origin/master`

`(branch-name) $ ./migrate.sh`

`(branch-name) $ git commit -am 'Message'`

`(branch-name) $ git push -f`