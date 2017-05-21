## Configurações do Apache 

Inserir as seguintes diretivas no ambiente VirtualHost:
  
    # /etc/apache2/sites-enabled/000-default.conf
    RewriteEngine On
    RewriteOptions inherit
    <Directory /var/www/html>
      Options All
      Allowoverride All
    </Directory>

Habilita módulo rewrite e restartar o apache:

    a2enmod rewrite
    service apache2 restart
