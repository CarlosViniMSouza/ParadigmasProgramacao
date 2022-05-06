## O que é programação orientada a objetos?

A POO é um paradigma de programação que se propõe a abordar o design de um sistema em termos de entidades, os objetos, e relacionamentos entre essas entidades. 

Imagine que estamos desenhando um sistema de gerenciamento de funcionários para uma empresa: o funcionário, sob esta abordagem, será uma entidade, e ele deve pertencer a um departamento. 

O departamento também será uma entidade, um objeto. Um departamento pode ter um ou mais funcionários. Logo, estabelecemos um relacionamento entre funcionário e departamento. 

Este funcionário pode ser terceirizado ou direto. Com isso, estabelecemos uma generalização, o funcionário, e sua especialização, ou seja, o funcionário terceirizado, por exemplo.

## Qual a diferença entre programação orientada a objetos e programação estruturada?

Na programação estruturada, a abordagem utilizada para o desenvolvimento de sistemas é procedural, ou seja, pensamos em um programa de computador como uma rotina ou sequência lógica, com início e fim determinados. 

Os programas são usados para processar uma entrada, alterando seus dados até que a saída desejada seja produzida. 

A programação estruturada é composta por três tipos de estruturas básicas: **sequências** (os comandos a serem executados), **condições** (blocos de decisão) e **repetições** (sequências que devem ser repetidas até chegar a determinada condição).

Esta abordagem pode se tornar problemática à medida em que os sistemas começam a ficar complexos. O acesso à variáveis se torna um problema, pois sub-rotinas devem compartilhar essas variáveis para processá-las. 

O reuso de rotinas fica muito difícil, na programação estruturada, obrigando códigos que desempenham essencialmente a mesma função tenham de ser reescritos. 

A legibilidade e a organização do código também é prejudicada, pois os programas passam a ficar muito longos e praticamente ilegíveis.

Na orientação a objetos, por outro lado, uma variável será vista como um atributo de um objeto, algo que ele “tem”. Um funcionário tem um nome. As funções passarão a ser as responsabilidades do objeto.

Se quisermos uma lista dos funcionários de um departamento, a função que retorna esses dados será responsabilidade da classe Departamento.

Mais à frente, vamos entender estas e mais características da programação orientada a objetos e como ela facilita o desenvolvimento de sistemas conceitualmente mais próximos da situação do mundo real que pretendemos modelar. 

## Quais são os 4 pilares da programação orientada a objetos?

A orientação a objetos, como vimos, é um modo de projetar e escrever um programa de modo a pensar nas entidades envolvidas como objetos que possuem características (os atributos) e responsabilidades (as funções) e estabelecer relações entre esses objetos. 

Ela tem quatro pilares principais: 

### Abstração

Consiste em extrair entidades do mundo real para dentro do código seguindo a fio suas responsabilidades. Um objeto deve ter uma identidade única dentro de um sistema, não podendo haver repetições.

Suas qualidades e responsabilidades devem ser bem definidas. Por exemplo:

Ao criar um estoque de itens em uma loja virtual, um produto teria como "qualidade" ou "características" um "nome", "categoria", "quantidade", etc. O mesmo produto também teria como “responsabilidade” ou “funcionalidade” o ato de diminuir ou aumentar a quantidade de itens no estoque, ou até o ato de ser removido do estoque por completo.

### Encapsulamento

Quando definimos os atributos de um objeto, devemos garantir que alterar os valores desses atributos sejam responsabilidade exclusiva do próprio objeto. O encapsulamento, portanto, é o conceito de proteger os atributos de um objeto. 

Em programação orientada a objetos, os atributos de um objeto são "trancados" dentro do objeto, definindo suas propriedades como privadas, ou seja, elas podem ser consultadas, mas não modificadas por outros objetos. 

### Herança

Para evitar repetição de entidades, usamos 'Herança' para passar características e responsabilidades. Em um sistema desenvolvido para uma escola, por exemplo, onde existam entidades "Alunos" e "Pessoas": Ao criar uma entidade (classe) Pessoa, podemos afirmar que toda pessoa possui um “nome”. Por outro lado, todo aluno também deveria ter um nome, sendo assim, para que todo Aluno tenha um nome, fazemos com que o Aluno, herde a característica “nome” de Pessoa, pois todo Aluno é uma Pessoa.

### Polimorfismo

O Polimorfismo, por sua vez, diz respeito à especialização das classes "filhas". Seguindo o Exemplo da Escola, a entidade Aluno teria como característica uma "matrícula", mesmo que a entidade Pessoa (pai de Aluno) não o tenha. Nesse caso, podemos afirmar que Aluno ainda teria sua base vinda de Pessoa, mas teria mudanças para sua funcionalidade específica.

Seguindo o mesmo padrão, poderia haver uma terceira entidade chamada "Professor", que seria herdada de Pessoa, mas com características diferentes de Alunos.

## Qual a importância da programação orientada a objetos?

Existem várias vantagens de se usar o paradigma de orientação a objetos na linguagem escolhida. Conheça as seis principais:

### Confiável

A orientação a objetos confere aos sistemas maior clareza, distribuição mais adequada de responsabilidades, encapsulamento de atributos e comportamentos, dentre muitas outras características. Isso torna o código mais seguro e confiável. 

### Oportuno

Por se aproximar mais do mundo real, modelando objetos reais e seus comportamentos, bem como o relacionamento entre esses objetos, a orientação a objetos é mais adequada ao desenvolvimento de software moderno.

### Ajustável

Ao concentrar em objetos atributos e funcionalidades, é bem mais fácil manter um código orientado a objetos. 

Se um sistema não se comporta da maneira esperada, torna- se mais fácil localizar o problema. 

### Extensível

A herança e o polimorfismo permitem a inclusão de funcionalidades em um sistema de forma muito direta. 

Suponha que um novo tipo de funcionário tenha de ser adicionado na nossa Escola, como por exemplo “Bibliotecário”. Grande parte da lógica dessa nova entidade já estará concentrada e encapsulada dentro da entidade Pessoa, restando apenas adicionar as características específicas dessa classe filha. 

### Reutilizável

Ao deslocar as funcionalidades do software de procedures para dentro de objetos, é possível, de forma muito fácil reutilizar código. 

Dentro do fluxo do código, sempre que é preciso desempenhar uma determinada tarefa, basta criar uma instância de um objeto que tenha aquela responsabilidade e invocar o método desse objeto. 

### Natural

A modelagem de software orientada a objetos aproxima o software do mundo real, tornando a engenharia de software uma questão de relacionar as entidades do mundo real com as ferramentas das quais o desenvolvedor dispõe na linguagem de programação escolhida. 