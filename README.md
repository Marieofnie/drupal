# Drupal via DDEV

## Local Setup

- make sure you have DDEV + Docker installed and running
- > ddev start (containers will start running)
- > ddev composer install (PHP dependencies will be downloaded)

- > ddev drush sql-drop -y
- > ddev drush sql-cli <dumps/dump.sql

- > ddev launch (site will be launched)

## Dumps

-when ready yopu need to export db changes, perform:

- > ddev drush cr
- > ddev drush sql-dump --result-file=../dumps/dump.sql

and commit all changes to git.
