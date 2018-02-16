# DB Model Edits
update model and mapper
run:

    ./scripts/db/auto-revision.sh "Message"

open file created from above
delete everything you don't need

    ./migrate.sh   # same as alembic upgrade head

go to tab 9 (DB) to make sure it is updated

    desc locations\G
    
test downgrade

    alembic downgrade -1
    desc locations\G   # check again in DB

reupgrade

    ./migrate.sh

