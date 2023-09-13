## Como configurar Laravel, Nginx, Redis e MySQL com Docker Compose
## Passo 1 — Fazendo download do Projeto e instalando dependências

Primeiramente, verifique se você está no seu diretório home e faça uma cópia da versão mais recente do Projeto para um diretório chamado environment:

    $ cd ~
    $ git clone git@github.com:acarlosos/environment-mydigitalstickers.git

Vá até o diretório environment-mydigitalstickers:

    $ cd ~/environment-mydigitalstickers

Vamos fazer uma cópia do arquivo .env.example para .env e inserir as configurações do banco de dados, redis e variaveis do docker:

    $ cp .env.example .env


Em seguida vamos clonar o projeto app-mydigitalstickers na pasta www

    $ cd www
    $ git clone git@acarlosos/app-mydigitalstickers .

Hora de levantar os containers:

    $ cd ..
    $  docker-compose up -d --build
