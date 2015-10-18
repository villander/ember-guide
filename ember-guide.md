## Conceitos Fundamentais

Para começar com Ember.js, há alguns conceitos que você precisa entender.

Ember.js foi projetado para ajudar desenvolvedores construirem grandes aplicações web que seja competitivas com os aplicativos nativos. Fazer isso requer novas ferramentas e um novo vocabulário de conceitos.

Contudo, é importante relembrar o que faz da web algo especial. Muitas pessoas pensam que algo é uma aplicação web porque ela usa HTML, CSS e JavaScript. Na realidade isto é apenas detalhes de implementação.

### Conceitos

#### Templates

O **template**, escrito em Handlebars templating language, descreve a interface do usuário de sua aplicação. Cada template é apoiado por um `model`, e o template autaliza automaticamente se o modelo muda.

Além do simples HTML, templates podem conter:

- **Expression**, como `{{firstName}}` que leva informações do model e coloca no HTML.

- **Outlets**, renderiza o template baseado na rota determinado pelo `router`. Baseado na rota o `controller` e a `view` correspondentes são utilizados. Isto é últil ao renderizar conteúdo baseado na rota, que é o caso mais comum.

- **Components**, elementos HTML customizados que você pode usar para limpar templates repetitivos ou criar controles reusáveis.


#### Router

O `router` traduz a URL para uma série de templates aninhados, cada um apoiado por um `model`. A medida que os templates e models estão sendo mostrado para a mudança do usuário, A Ember mantém automaticamente a URL na barra de endereços do navegador `up-to-date`.

Isto significa que, em qualquer ponto, os usuários são capazes de compartilhar a URL do seu aplicativo. Quando alguém clica no link, eles veêm de maneira confiável o mesmo conteúdo que o usuário original.

#### Components

O **component** é um tag HTML customizada cujo comportamento você implementa usando JavaScript e cuja aparência você descreve usando Handlebars templates. Ele permique que você crie controles reusáveis que você pode simplificar os templates de sua aplicação.

#### Models

O **model** é o objeto que armazena o  *persistent state*. Templates são responsáveis por mostra o model para o usuário por transformá-lo em HTML. Em muitas aplicações, models são carregados em `HTTP JSON API`, embora Ember é agnóstica para o servidor que você escolher.

#### Routes

A **rota** é o objeto que diz ao template que `model`ele deve exibir.

---------------------------

Estes são os conceitos fundamentais que você precisa entender para desenvolver sua Ember.js app. Ela é projetada para escalar em termos de complexidade. De modo que a adição de novas funcionalidades não vai te forçar a voltar atrás e refazer as principais partes da sua app.

Agora que você entende o papel desses objetos, você está equipado para mergulhar profundamente em Ember.js e aprender os detalhes de como cada uma dessas peças individuais trabalham.


