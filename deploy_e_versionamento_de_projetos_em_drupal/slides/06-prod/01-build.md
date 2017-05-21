## Subindo ambiente de produção: 

Clone:
   
    cd ~
    git clone desenvolvimento producao

Provisionamento:   

    u='fatec666_prod'
    cd producao
    composer install
    cd web
    ../vendor/bin/drush si --db-url=mysql://$u:$u@127.0.0.1/$u --account-name="${u}" --account-pass="${u}" --site-name="produção" -y

Ativar a feature movie_reviews:

    ../vendor/bin/drush en features -y
    ../vendor/bin/drush en movie_reviews -y
