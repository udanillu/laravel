<img src="images/laraveltop.jpg" alt="Laravel Banner">

> Status: Developing 

Esse repositório foi criado com o intuito de ensinar a como criar uma Aplicação de Login, com as tecnologias ![Laravel](https://laravel.com/) | ![Breeze](https://laravel.com/docs/9.x/starter-kits), irei disponibilizar os comando & links para o desenvolvimento do projeto. Não só isso, ensinarei como fazer upload da aplicação em uma Plataforma Cloud chamada ![Heroku](https://www.heroku.com/), usando a ferramenta ![Git](https://git-scm.com/downloads).

### Instalações Necessárias ☑️ 

+ ![PHP](https://www.apachefriends.org/pt_br/index.html)
+ ![Composer](https://getcomposer.org/Composer-Setup.exe) 
+ ![Git](https://git-scm.com/downloads)
+ ![Heroku](https://devcenter.heroku.com/articles/heroku-cli)
+ ![NPM](https://nodejs.org/en/)
```bash 
$ composer global require laravel/installer
```

### Desenvolvimento 🎲

```bash
# Abrir Terminal/CMD
$ composer create-project laravel/laravel NomeDoSeuProjeto --prefer-dist
# Acesse o Projeto no Terminal/CMD
$ cd NomeDoSeuProjeto

# Configurar um Banco de Dados (MySQL, SQLITE e ou Firebase)
$ php artisan migrate

# Instale Breeze nas Dependências 
$ composer require laravel/breeze --dev
$ php artisan breeze:install

# Testar Login | Registro
$ npm install
$ npm run dev
# Abrir Outro Terminal/CMD
$ php artisan serve
```

Caso você já consiga acessar o seu projeto e esteja conseguindo se cadastrar, vamos ao próximo passo, dar Git Init no projeto e enviá-lo ao ![Heroku](https://www.heroku.com/), para que todos possam acessar o projeto. É um processo essencial, exigindo atenção. 

### Git Init Heroku 🧙‍♂️

```bash
# Iniciar o Git 
$ git init
# Adicinar Pastas
$ git add .
# Configurar Usuário
$ git config --global user.email "SeuEmail@gmail.com"
$ git config --global user.name "SeuNome"
# Commitar
$ git commit -am "First Commit"
$ git remote -v
# Logar com Heroku
$ heroku login -i
# Criar Cloud (não pode ter letras maiúsculas)
$ heroku create nomedoprojeto
# Criar um arquivo "Procfile", fora do Terminal/CMD
web: vendor/bin/heroku-php-apache2 public/
# Adicionar Mudanças
$ git add .
# Commitar Mudanças
$ git commit -am "Procfile"
# Ver o nome da Brach (minha branch é a master)
$ git branch
# Enviar para Heroku
$ git push heroku master
# Últimas Configurações
$ heroku config:set APP_DEBUG=true
# Gerar Key
$ php artisan key:generate --show
# Definir Key, depois do =, colocar a key gerada acima
$ heroku config:set APP_KEY=
# Abrir Projeto
$ heroku open
```

pós ter desenvolvido todos os comandos, você será capaz de ver a sua aplicação rodando em um ambiente Cloud, conseguindo disponibilizar o link de acesso para seus colegas. Um exemplo de um site hospedado no ![Heroku](https://devcenter.heroku.com/articles/heroku-cli) é um ![Gerador de Nomes](https://gerador-nomes.herokuapp.com), que é hospedado grátis. Na tabela abaixo, nós podemos ver as versões das tecnologias usadas. 

<br>

<table align="center">
  <tr>
    <td>Composer</td>
    <td>Heroku</td>
    <td>Laravel</td>
    <td>Breeze</td>
    <td>Git</td>
  </tr>
  <tr>
    <td>2.3</td>
    <td>7.6</td>
    <td>4.2</td>
    <td>1.1</td>
    <td>2.3</td>
  </tr>
</table>

<br>

### Como Rodar a Minha Aplicação?

```bash
$ npm install
$ npm run dev
# Abrir outro Terminal/CMD
$ php artisan serve
```

<br>

<a href="https://www.linkedin.com/in/danillucruz/" alt="LinkedIn">
  <img src="images/linkedin.jpg" align="center" alt="LinkedIn">
</a>



