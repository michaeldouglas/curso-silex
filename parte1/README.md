## Silex Curso - Parte 1 - Baixando o Bootstrap

Para baixar o Framework Bootstrap utilizaremos o Bower que é um 
gerenciador de componentes de front-end que pode ser utilizado
em qualquer projeto até mesmo o nosso que é PHP!

Para saber mais sobre o projeto acesse o link: [bower.io](bower.io)

## Instalação

Para instalar o Bower no projeto basta você executar em seu terminal
o link:

```
npm install -g bower
```

## Instalação do Bootstrap

O nosso projeto já está configurado com o `bower.json` que fica
responsável por verificar as dependências do projeto e instalar!

Sendo assim basta você executar o comando:

```
bower install
```

Ou apenas:

```
bower i
```

Jovem padawan:

![](http://st-peters.bournemouth.sch.uk/tlplus/wp-content/uploads/2014/01/Yoda-and-Luke-620x410.jpg)

Lembrar você deve de não comitar a `bower_components`

## Ajuste da pasta do projeto

Iremos então criar um arquivo na estrutura chamado: `.bowerrc` 
que contém em sua estrutura um ajuste para como desejamos
que nossos pacotes estejam:

```
{
  "directory": "assets/vendor/"
}
```

Em seguida delete a pasta chamada: `bower_components` e execute
novamente o comando:

```
bower i
```

Repare que a pasta agora mudou para: `assets` isso por que 
configuramos no arquivo `.bowerrc` para que ele mantenha nesse
padrão.

## Testando o Layout

Para testar nosso Layout use o código:

```html
<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Curso Silex PHP Conference</title>

    <link href="assets/vendor/bootstrap/dist/css/bootstrap.min.css" rel="stylesheet">

    <!--[if lt IE 9]>
    <script src="https://oss.maxcdn.com/html5shiv/3.7.2/html5shiv.min.js"></script>
    <script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
    <![endif]-->
</head>
<body>

<div class="panel panel-default">
    <div class="panel-heading">Silex</div>
    <div class="panel-body">
        PHP Conference
    </div>
</div>

<script src="assets/vendor/jquery/dist/jquery.min.js"></script>
<script src="assets/vendor/bootstrap/dist/js/bootstrap.min.js"></script>

</body>
</html>
```
## Formulário de contato

iremos alterar nosso HTML inclunindo o bloco do formulário, mas veja 
não iremos criar o envio e validações pois é apenas um exemplo:

```html
<div class="panel panel-default">
    <div class="panel-heading">Silex</div>
    <div class="panel-body">
        <form>
            <div class="form-group">
                <label for="exampleInputEmail1">Email</label>
                <input type="email" class="form-control" id="exampleInputEmail1" placeholder="Email">
            </div>
            <div class="form-group">
                <label for="exampleInputPassword1">Nome</label>
                <input type="text" class="form-control" id="exampleInputPassword1" placeholder="Nome">
            </div>
            <button type="submit" class="btn btn-default">Enviar</button>
        </form>
    </div>
</div>
```
