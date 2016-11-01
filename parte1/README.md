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

## Ajuste do nome da pasta

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