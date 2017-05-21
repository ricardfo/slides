## Banco de dados MySQL

Banco de dados desenvolvimento: 

    create database thais_dev;
    grant all privileges on thais_dev.* to thais_dev@'%'  identified by 'thais_dev';

Banco de dados produção: 

    create database thais_prod;
    grant all privileges on thais_prod.* to thais_prod@'%' identified by 'thais_prod';
