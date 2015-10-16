# ember-testing

## Introduçao

Teste é uma parte essencial do framework Ember e seu ciclo de desenvolvimento .


Vamos assumir que estamos trabalhando em uma aplicacao Ember que servira como um blog. Esta aplicacao provavelmente incluira `models` para `users` e `posts`. Isto tambem devera incluir interacoes para `login` e `create` post. Vamos finalmente assumir que voce quer ter [testes automatizados](https://en.wikipedia.org/wiki/Test_automation) em sua aplicacao.

Ha dois tipos de classificacoes diferentes de testes que voce ira precisar: **Aceitacao** e **Unitario**.

### Teste de Aceitacao

Teste de aceitacao sao usados para testar interacao do usuario e o fluxo da  aplicacao. Considerando  nosso cenario do blog alguns testes que voce pode escrever sao:

 - Um usuario eh capaz de fazer login atraves de um formulario de login
 - Um usuario eh capaz de criar um post no blog
 - O visitante nao pode ter acesso ao painel de administracao
 
### Teste Unitario

Testes unitarios sao usados para testar pedacos de funcionalidades, ou " unidades" sem se preocuupar com  suas dependencias. Considerando  nosso cenario do blog alguns testes que voce pode escrever sao:

 - O usuario tem uma permissao
 - O usuario tem um username
 - O usuario tem um nome completo que eh agregado do seu primeiro e ultimo nome com espaco entre os dois
 - O post tem um titulo
 - O titulo de um post nao pode ter mais que 50 caracteres
 
### Framework de Teste

[QUnit](http://qunitjs.com/) eh o framework de teste padrao do Ember, e  iremos usa-lo neste guia . Mas outros tambem sao suportados atraves de `addons` de terceiros

### Como rodar seus testes
