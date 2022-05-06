## O que é programação funcional?

Podemos conceituar a programação funcional como um paradigma de desenvolvimento, assim como outros já bem estabelecidos no mercado hoje:

&nbsp; &nbsp; ° programação orientada a objeto;

&nbsp; &nbsp; ° programação imperativa;

&nbsp; &nbsp; ° programação estruturada.

Mesmo que esses exemplos sejam os mais famosos, aqueles pelos quais aprendemos programação em cursos e faculdades, existem outros paradigmas utilizados em algumas aplicações e casos específicos.

Podemos dizer que o paradigma na programação é **a organização do código e de todas as suas ferramentas como funções e variáveis**.

Na orientação a objetos, por exemplo, as funções e os dados serão modelados pensando em entidades do mundo real, com características e comportamentos espelhados de objetos.

Já na imperativa, temos uma sequência de passos simples com o objetivo único de resolver um problema específico.﻿ O que seria então o paradigma funcional dentro desse contexto? E quais são suas especificidades? Vamos descobrir.

O paradigma funcional não dita diretamente o código e suas responsabilidades. Dividimos todo o processo de transformação de dados em funções complementares, que fazem, cada uma de uma vez, parte do processamento para resolver o problema.

Podemos simplificar dizendo que **um código escrito sob um paradigma funcional é composto de múltiplas funções, que trabalham de forma unificada para a resolução de um problema**. Entender e aplicar esse modelo pode ser uma ótima oportunidade profissional.

## Quais os principais conceitos da programação funcional?

Existe uma série de conceitos dentro da programação funcional que devem ser utilizados para que possamos aplicar a definição de forma correta. Vamos listar cada um deles com exemplos.

Utilizaremos o Javascript para os códigos, mas você pode usar qualquer linguagem de sua preferência.

### Composição de Função

Chamamos de composição de funções a criação de uma nova função por meio de uma junção de outras, realizando mais de uma atribuição em uma única chamada.

No exemplo abaixo, vamos criar um array com alguns algarismos e, depois disso, filtraremos apenas os números pares e multiplicaremos por 2:

```js
const algarismos = [2, 3, 4, 5, 6, 7, 8, 9, 10]

algarismos.filter((numero) => numero % 2 === 0).map((numero) => numero * 2) 

// [ 4, 8, 12, 16, 20 ]
```

### Funções Puras

Chamamos de função pura todas as funções que, quando invocadas mais de uma vez, produzem exatamente o mesmo resultado. Ou seja, independentemente dos valores passados para a função, que podem até mesmo ser mutáveis, o valor retornado deve sempre ser o mesmo.

Contudo, é preciso atenção, pois ela não pode causar efeitos colaterais externamente. Caso o resultado seja mutável, o comportamento do restante do sistema pode ser imprevisível, levando a erros e falhas.

Vamos ver um exemplo bem simples:

```js
const verfica_se_eh_menor_que = (var1, var2) => var1 <= var2;
```

A saída da função poderia ser:

```js
verfica_se_eh_menor_que(9, 13) 
// output: true
```

A função acima atende aos requisitos de uma função pura, pois seu resultado sempre será true ou false. Assim, ela pode ser executada em paralelo com as demais sem nenhum tipo de problema ou sem gerar falhas.

### Imutabilidade

O conceito de imutabilidade na programação significa que uma variável, que ao longo do código foi carregada com um valor, vai manter esse valor enquanto o programa estiver sendo executado, sem voltar a mudar seu estado.

Chamamos isso de constante, sendo que cada linguagem trabalha de uma forma diferente com esse tipo de variável. No Javascript, podemos utilizar dessa maneira:

```js
const numeroUnico = 34

numeroUnico = 27

console.log(numeroUnico) // 34
```

Ao imprimirmos a constante, mesmo que tenhamos tentado mudar seu valor, poderíamos ver que ela continua a mesma.

## Efeito Colateral

Dentro do paradigma de programação funcional, o efeito colateral corresponde a toda interação com o mundo externo, ou seja, fora do sistema. São ações como:

&nbsp; &nbsp; ° alterar dados no banco;

&nbsp; &nbsp; ° comunicação com APIs;

&nbsp; &nbsp; ° alterar propriedades de objetos.

Logo acima falamos sobre a questão de funções puras não causarem nenhum tipo de efeito colateral. E agora aqui estamos nós falando que efeito colateral é um dos conceitos de programação funcional. Calma, vamos explicar!

No desenvolvimento de software, os dados mudam de forma constante, e isso não pode ser evitado totalmente. O que fazemos então, dentro da programação funcional, é tentar isolar e confinar o efeito colateral.

Podemos dizer que esses pontos de contato serão as funções impuras, pois serão separados do restante do código e deverão lidar com interfaces de comunicação, levando e trazendo valores mutáveis.

## Estado Compartilhado

Por fim, temos o que chamamos de estado compartilhado, que nada mais são que valores que podem ser acessados em mais de um ponto da aplicação. Vamos ao exemplo:

```js
const idade = 31

const calculaIdadeDosAmigos = ( idadeAmigo ) => idade + idadeAmigo
```

Aqui, a função utiliza uma variável externa — a nossa constante, lembra? —, que não está listada dentro de seu escopo, mas que pode ser acessada normalmente. Ou seja, não precisamos passá-la dentro dos argumentos de chamada da função.

## Vantagens e desvantagens

Caso você pergunte a pessoas programadoras mais experientes para o que usariam a programação funcional, a resposta seria para aplicar, na prática, alguns pensamentos matemáticos, porém esse é um paradigma que vai além.

Muitos de nossos problemas diários poderiam ser resolvidos com base no modelo funcional, por exemplo, processamento paralelo — algo que pode ser muito difícil para outros paradigmas como o orientado a objetos.

Além disso, um **código funcional é muito mais conciso, simples e sem floreios**, o que facilita as pessoas programadoras realizarem manutenções e entender trechos escritos por outros programadores rapidamente.
