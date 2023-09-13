## Como configurar Laravel, Nginx, Redis e MySQL com Docker Compose
## Passo 1 — Fazendo download do Projeto e instalando dependências

Primeiramente, verifique se você está no seu diretório home e faça uma cópia da versão mais recente do Projeto para um diretório chamado environment:

    $ cd ~
    $ git clone git@github.com:acarlosos/environment.git

Vá até o diretório environment:

    $ cd ~/environment

Vamos fazer uma cópia do arquivo .env.example para .env e inserir as configurações do banco de dados, redis e variaveis do docker:

    $ cp .env.example .env

Crie o diretório www:

    $ mkdir www

Em seguida vamos clonar o projeto aplicacao-web

    $ git clone git@seuprojeto.com.br .

Hora de levantar os containers:

    $ docker-compose up -d --build
