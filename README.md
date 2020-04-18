<h1 align="center">
  <img alt="Fastfeet" title="Fastfeet" src="./backend/img/logo.png" width="300px" />
</h1>

<h3 align="center">
  Fastfeet Application 🚚 🛵 🚴 📦
</h3>

<p align="center">

  <a href="https://app.codacy.com/manual/kaiorr/gostack-fastfeet?utm_source=github.com&utm_medium=referral&utm_content=kaiorr/gostack-fastfeet&utm_campaign=Badge_Grade_Settings">
    <img alt="Code Covarage" src="https://api.codacy.com/project/badge/Grade/880f947032d543fa913769c4313a9bb1">
  </a>

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

## 🚀 Sobre o desafio

A aplicação de um app para uma transportadora fictícia, o FastFeet, é uma aplicação completa envolvendo back-end, front-end e mobile, que será utilizada para a **certificação do bootcamp** Gostack da **[rocketseat](https://rocketseat.com.br/gostack)**.

# Iniciando o Servidor Backend

>Instalação do NodeJS e Docker:

## 📦 Node

>Para instalar via terminal linux Ubuntu, digite o comando:
> -  Using Ubuntu
> -  curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -sudo apt-get install -y nodejs

Caso tenha interesse segue a lista completa de instalação para as demais distros suportadas pelo Nodejs, basta [acessar](https://github.com/nodesource/distributions/blob/master/README.md) o repositório do projeto

## 🐳 Docker

Para instalação do Docker é necessário acesssar a [documentação](https://docs.docker.com/install/linux/docker-ce/ubuntu/), nesse caso seguindo o padrão ubuntu. Basta seguir o passo a passo para instalação.

## Pós instalação Docker

Para utilizar o docker, subir imagens, gerenciamento, sem a nessecidade de utilizar o root, basta seguir o link para [documentação](https://docs.docker.com/install/linux/linux-postinstall/), onde é demonstrado o passo a passo para utilização do docker com user da máquina.

### ⏯ Acesssando

> -  git clone https://github.com/kaiorr/gostack-fastfeet.git
> -  cd gostack-fastfeet

### Instalando todos pacotes

> yarn

> Criando as bases de dados (Postgres):
> -  docker run --name fastfeet -e POSTGRES_PASSWORD=fastfeet -p 5432:5432 -d postgres
> -  docker start fastfeet

> Criando base de dados Redis:
> -  docker run --name redisfastfeet -p 6379:6379 -d -t postgres
> -  docker start redisfastfeet

> Instalando o PostBird, para utilização da base de dados de forma visual:
> -  sudo snap install postbird
> Quando acessar o postbird informar os dados de acesso, host, port, username e password definidos na criação via docker.
> -  criar banco com nome fastfeet

### 🔑 .env

> -  Alterar o arquivo .env e informar todos parâmetros.
> -  Para definir a secret corretamente, basta acessar o site do MD5 clicando, [aqui](https://www.md5online.org/) e informar a secret abaixo e alterar no .env o hash.
> -  **APP_SECRET=bootcampgostackfastfeetkaioribeiro**

### ☑ Criando a migrations

> yarn sequelize db:migrate

### ☑ Criando Seeds

> yarn sequelize db:seed:all

## 🔛 Subindo servidor

> yarn dev

## 🔛 Subindo servidor de email

> yarn queue

# 💻 Iniciando o Frontend

> Para instalar as dependências
> -  yarn
  
> Para subir aplicação
> -  yarn start


# 📱 Mobile

> :heavy_plus_sign:  **Aplicativo testado somente Android**
> Para instalar as dependências 
> -  yarn
> -  :pushpin:  Foi utilizado Genymotion como emulador android, para maiores informações do mesmo, basta seguir o guia de instalação e configuração disponibilizado **[aqui](https://docs.rocketseat.dev/ambiente-react-native/android/emulador)** toda documentação criado pela rocketseat para auxíliar no processo de criação do ambiente.

## 🔛 Iniciando App

> -  yarn start
> -  react-native run-android

## 🤔 Como Contribuir

**Encare essa contribuição como uma forma de consolidar seu conhecimento sobre git e gitbub, todo e qualquer feedback será bem vindo.**

> -  Faça fork do repositório
> -  Crie uma nova branch **git checkout -b my feature**
> -  Faça um commit **git commit -m "feat: My new feature"**
> -  Envie sua branch para seu repositório forkado **git push origin my feature**
> -  Crie um novo Pull Request informando sobre suas alterações e aguarde para obter reposta sobre o mesmo.

## 📝 Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](https://raw.githubusercontent.com/kaiorr/gostack-fastfeet/master/LICENSE) para mais detalhes.

----

Feito com :heart: por **Kaio Ribeiro** :call_me_hand: [Professional Network](https://www.linkedin.com/in/kaio-ribeiro-310123150/)
