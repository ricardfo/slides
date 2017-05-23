## Preparação da infraestrutura: 

Instalação das dependências em ambiente (debian 8):
   
    sudo apt-get -y install php php-xml php-intl php-mbstring 
    sudo apt-get -y install php-pgsql
    #apt-get install vim php php5-gd php5-mysql git drush mysql-server

Instalação do symfony: 

    sudo curl -LsS https://symfony.com/installer -o /usr/local/bin/symfony
    sudo chmod a+x /usr/local/bin/symfony

Baixar composer:

    wget https://getcomposer.org/installer
    php installer
    mv composer.phar /usr/local/bin/composer
    rm installer

Criar um usuário no grupo www-data:

    useradd -m -d /var/www/html/thais -s $(which bash) -G www-data  thais
    echo thais:123 | chpasswd
