<h1 align="center">
  <img alt="Fastfeet" title="Fastfeet" src="./backend/img/logo.png" width="300px" />
</h1>

<h3 align="center">
  Fastfeet Application :package:
</h3>

<p align="center">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/kaiorr/aceleraDevReact?style=plastic">

  <a href="https://www.linkedin.com/in/kaio-ribeiro-310123150/"> 
    <img alt="Made by Kaio" src="https://img.shields.io/badge/made%20by-kaiorr-%2304D361">
  </a>

  <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/kaiorr/aceleraDevReact?color=7800ff&style=plastic">

  <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/kaiorr/aceleraDevReact?color=7800ff&style=plastic">

  <a href="https://github.com/kaiorr/aceleraDevReact/stargazers">
    <img alt="Stargazers" src="https://img.shields.io/github/stars/kaiorr/aceleraDevReact?style=social">
  </a>
</p>

<p align="center">
  <a href="#rocket-sobre-o-desafio">Sobre o desafio</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#iniciando-o-servidor-backend">Backend</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#computer-iniciando-o-frontend">Frontend</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#iphone-mobile">Mobile</a>
</p>

## :rocket: Sobre o desafio

A aplicação de um app para uma transportadora fictícia, o FastFeet, é uma aplicação completa envolvendo back-end, front-end e mobile, que será utilizada para a **certificação do bootcamp** Gostack da **[rocketseat](https://rocketseat.com.br/gostack)**.

# Iniciando o Servidor Backend

Instalação do NodeJS e Docker:

## :package: Node

Para instalar via terminal linux Ubuntu, digite o comando:

    # Using Ubuntu
    curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
    sudo apt-get install -y nodejs

Caso tenha interesse segue a lista completa de instalação para as demais distros suportadas pelo Nodejs, basta [acessar](https://github.com/nodesource/distributions/blob/master/README.md) o repositório do projeto

## :whale2: Docker

Para instalação do Docker é necessário acesssar a [documentação](https://docs.docker.com/install/linux/docker-ce/ubuntu/), nesse caso seguindo o padrão ubuntu. Basta seguir o passo a passo para instalação.

## Pós instalação Docker

Para utilizar o docker, subir imagens, gerenciamento, sem a nessecidade de utilizar o root, basta seguir o link para [documentação](https://docs.docker.com/install/linux/linux-postinstall/), onde é demonstrado o passo a passo para utilização do docker com user da máquina.


### :zap: Acesssando

    git clone https://github.com/kaiorr/gostack-fastfeet.git

  Acessando o diretório:

      cd gostack-fastfeet

  Instalando todos pacotes:

      yarn

  Criando as bases de dados (Postgres):

      docker run --name fastfeet -e POSTGRES_PASSWORD=fastfeet -p 5432:5432 -d postgres
      docker start fastfeet

  Criando base de dados Redis:

      docker run --name redisfastfeet -p 6379:6379 -d -t postgres
      docker start redisfastfeet


  Instalando o PostBird, para utilização da base de dados de forma visual;

      sudo snap install postbird

  Quando acessar o postbird informar os dados de acesso, host, port, username e password definidos na criação via docker.

      criar banco com nome fastfeet

### :key: .env

  Alterar o arquivo .env.example para .env e informar todos parâmetros.

  Para definir a secret corretamente, basta [acessar](https://www.md5online.org/), informar a secret abaixo e alterar no .env o hash.

      APP_SECRET=bootcampgostackfastfeetkaioribeiro

### :white_check_mark: Criando a migrations

    yarn sequelize db:migrate

### :white_check_mark: Criando Seeds

    yarn sequelize db:seed:all

## :on: Subindo servidor

    yarn dev

## :on: Subindo servidor de email

    yarn queue

# :computer: Iniciando o Frontend

  Para instalar as dependências

      yarn
  
  Para subir aplicação

      yarn start


# :iphone: Mobile

:heavy_plus_sign:  **Aplicativo testado somente Android**

    Para instalar as dependências 

        yarn

:pushpin:  Foi utilizado Genymotion como emulador android, para maiores informações do mesmo, basta seguir o guia de instalação e configuração disponibilizado **[aqui](https://docs.rocketseat.dev/ambiente-react-native/android/emulador)** toda documentação criado pela rocketseat para auxíliar no processo de criação do ambiente.

## Iniciando App

    yarn start

    react-native run-android

## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para mais detalhes.

----

Feito com :heart: por **Kaio Ribeiro** :call_me_hand: [Professional Network](https://www.linkedin.com/in/kaio-ribeiro-310123150/)
