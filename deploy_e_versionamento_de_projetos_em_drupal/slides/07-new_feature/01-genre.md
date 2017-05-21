## Alterando o projeto

No ambiente de desenvolvimento, adicinar um novo gênero de filme: *romance* e 
re-exportar outra versão da feature. Commit na mudança:

    cd ~/desenvolvimento
    git status
    git add --all
    git commit -m 'adicinando novo gênero'

Aplicar mudança no ambiente de produção:

    cd ~/producao
    git pull origin master
    cd web
    ../vendor/bin/drush fd movie_reviews
    ../vendor/bin/drush features-import  movie_reviews -y
