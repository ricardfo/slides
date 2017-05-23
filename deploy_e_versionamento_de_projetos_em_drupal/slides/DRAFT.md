./vendor/bin/drupal server

./vendor/bin/drupal site:install --db-type='pgsql' --db-host='192.168.100.71' --db-name='drupal' --db-user='fflch' --db-pass='fflch' --db-port=5432 --site-name='Drupal' --site-mail='teste@usp.br' --account-name='admin' --account-mail='admin@exemplo.com' --account-pass='admin'


./vendor/bin/drupal generate:module

./vendor/bin/drupal module:install

http://127.0.0.1:8088/admin/structure/default_entity

