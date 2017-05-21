## Preparação da infraestrutura: 

Instalação das dependências em ambiente (debian 8):
   
    apt-get install vim php5 php5-gd php5-mysql git drush mysql-server

Baixar composer:

    wget https://getcomposer.org/installer
    php installer
    mv composer.phar /usr/local/bin/composer

Criar um usuário no grupo www-data:

    useradd -m -d /var/www/html/thais -s $(which bash) -G www-data  thais
    echo thais:123 | chpasswd
