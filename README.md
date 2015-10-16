# ember-testing

## Introduçao

Teste é uma parte essencial do framework Ember e seu ciclo de desenvolvimento .


Vamos assumir que estamos trabalhando em uma aplicacao Ember que servirá como um blog. Esta aplicação provavelmente incluirá `models` para `users` e `posts`. Isto também deverá incluir interações para `login` e `create` post. Vamos finalmente assumir que você quer ter [testes automatizados](https://en.wikipedia.org/wiki/Test_automation) em sua aplicação.

Ha dois tipos de classificacoes diferentes de testes que você irá precisar: **Aceitação** e **Unitário**.

### Teste de Aceitação

Teste de aceitação são usados para testar interacção do usuário e o fluxo da  aplicacao. Considerando  nosso cenario do blog alguns testes que você pode escrever são:

 - Um usuário é capaz de fazer login através de um formulário de login
 - Um usuário é capaz de criar um post no blog
 - O visitante não pode ter acesso ao painel de administracao

### Teste Unitário

Testes unitários são usados para testar pedacos de funcionalidades, ou " unidades" sem se preocuupar com  suas dependencias. Considerando  nosso cenario do blog alguns testes que você pode escrever são:

 - O usuário tem uma permissão
 - O usuário tem um username
 - O usuário tem um nome completo que é agregado do seu primeiro e último nome com espaco entre os dois
 - O post tem um titulo
 - O titulo de um post não pode ter mais que 50 caracteres

### Framework de Teste

[QUnit](http://qunitjs.com/) é o framework de teste padrao do Ember, e  iremos usá-lo neste guia . Mas outros também são suportados através de `addons` de terceiros

### Como rodar seus testes

Rode seus testes com o comando `ember test` na linha de comando.Você pode reexecutar os testes em cada arquivo de mudança com `ember test --server`. Para mais detalhes e opções, veja [Ember CLI – Testing](http://www.ember-cli.com/user-guide/#testing) ande `ember helper test`.

>>[Testes de Aceitação]()











