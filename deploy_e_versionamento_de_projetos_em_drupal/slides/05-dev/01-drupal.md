## Baixando e instalando Drupal

Baixar Drupal e módulo features usando o composer:

    composer create-project drupal-composer/drupal-project:8.x-dev desenvolvimento --stability dev --no-interaction
    cd ~/desenvolvimento
    composer require drupal/features

Ignorar arquivos de configuração:

    cd ~/desenvolvimento
    echo "web/sites/default/settings.php" >> .gitignore
    echo "web/sites/default/services.yml" >> .gitignore

Instalar drupal e habilitar módulo features:
 
    u='fatec666_dev'
    cd ~/desenvolvimento/web/
    ../vendor/bin/drush si --db-url=mysql://$u:$u@127.0.0.1/$u --account-name="${u}" --account-pass="${u}" --site-name="Desenvolvimento" -y
    ../vendor/bin/drush en features_ui -y
