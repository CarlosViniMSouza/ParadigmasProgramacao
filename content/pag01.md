## Programação imperativa

Para se entender o que é programação imperativa, vamos primeiramente voltar ao significado original deste termo na nossa amada, querida e difícil língua portuguesa:

```
Imperativo: que acentua o caráter de mando, de autoridade, 
ou que exprime uma ordem; autoritário.
```

Então, imperatividade dá a ideia de dar ordens ou se dizer com todas as letras o que se deve fazer a alguém. E pode-se dizer que programação imperativa possui ideia semelhante.

Baseado em instruções e comandos, o programador diz como e o quê exatamente um programa ou rotina deve realizar. É neste paradigma que surgiram os famosos laços de repetição, estruturas condicionais, atribuição de valor à variáveis e controle de estado.

A maioria de nós programadores utilizamos este paradigma de programação no nosso dia a dia sem, muitas vezes, nos darmos conta disto.

Instruções como **if**, **while**, **switch** e **for** são típicas de linguagens de programação imperativas.

## Programação declarativa

Uma das principais características do paradigma declarativo é que não há preocupação na maneira ou método de execução de uma determinada rotina. Em outras palavras, o foco não está no “como” e sim no “que”.

Por mais incrível que possa parecer, um dos principais exemplos de utilização de programação declarativa na nossa rotina de programador é a utilização da linguagem SQL. Quando especificamos uma simples instrução SELECT, simplesmente declaramos ao banco de dados o que queremos, sem necessidade de nos importarmos com os procedimentos que o gerenciador de banco de dados adotará para fazer funcionar corretamente a instrução. 

Esta característica torna o modo de programação declarativo muito mais simples e legível em comparação à programação imperativa.

Um dos principais exemplos atuais e consenso em relação aos benefícios da utilização de programação declarativa está preconizado no Angular, framework javascript que possui implementações declarativas.

Como exemplo, suponhamos que temos que implementar em uma página Web uma funcionalidade que, caso o usuário marque a opção de seleção em um controle do tipo checkbox, uma mensagem deve ser exibida, caso contrário, a mensagem deve ser ocultada.

Utilizando JQuery e o modo de programação imperativo, a implementação ficaria semelhante a isto:

![img01 - JQuerry](https://miro.medium.com/max/1400/1*B2M7vtFSq8LZe7pKZQGGMw.png)

Para a implementação funcionar conforme o desejado foi necessária a criação de uma função que possuísse a implementação, especificando de forma imperativa o que deveria acontecer no caso o estado do controle checkbox fosse alterado.

Caso decidíssemos utilizar Angular no nosso projeto, que possui um modo de programação declarativo, a implementação ficaria semelhante a esta:

![img02 - Angular](https://miro.medium.com/max/1384/1*4yn4V_RiikLNas-FKBO5zw.png)

Repararam na simplicidade? Possui exatamente o mesmo resultado da primeira implementação, mas com nenhuma linha de código adicional além do HTML. O modo de programação declarativa tem se mostrado bastante eficaz para front-end.

## Programação reativa

A programação reativa talvez não possa ser considerada um paradigma de programação como os demais citados, mas representa um conceito que tem sido amplamente utilizado nas aplicações Web modernas, onde pode haver uma complexidade extremamente alta das interações do usuário e a grande necessidade de disponibilidade das aplicações, exigindo grande performance de resposta e assincronismo. 

Em sistemas reativos a aplicação responde ou REAGE a eventos disparados por interações de usuário ou situações comuns em aplicações como falhas, sobrecarga de requisições, dentre outros, retornando apenas ao que foi solicitado e/ou respondendo de maneira adequada a cada situação.

Atualmente, escalabilidade é um pré-requisito cada vez mais fundamental ao se planejar a arquitetura de um sistema Web, considerando altas exigências por performance, tempo de resposta, processamento de grande quantidade de requisições simultaneamente, acesso de diversos dispositivos, dentre outras características. E é aí que entra a programação reativa, juntamente com outros conceitos como microservice, computação em nuvem, etc.

E para se definir e padronizar o conceito de sistemas reativos, foi criado o Manifesto Reativo, com alguns princípios referentes a este modo de projetar as aplicações: [The Reactive Manifest (in PT-BR)](https://www.reactivemanifesto.org/pt-BR)

Basicamente, os sistemas reativos precisam atender a quatro principais características: elasticidade, resiliência, responsividade e ser orientado a mensagens.

Para dar suporte a este paradigma foram criados ou adaptados alguns frameworks e bibliotecas, como o **React.js**, desenvolvido e mantido pelo Facebook, e que vem sendo utilizado por grandes empresas como o Netflix.
