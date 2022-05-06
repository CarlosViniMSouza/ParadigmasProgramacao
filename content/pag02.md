## Elementos Chaves da Programação Estruturada

A programação estruturada é uma forma de programação de computadores que estabelece uma disciplina de desenvolvimento de algoritmos, independentemente da sua complexidade e da linguagem de programação na qual será codificado, que facilita a compreensão da solução através de um número restrito de mecanismos de codificação.

1. Estruturas básicas de controle: sequência, condição e repetição.

São formas de raciocínio intuitivamente óbvias. A legibilidade e compreensão de cada bloco de código na solução é enormemente incrementada, proibindo o uso irrestrito de comandos de desvio incondicional (GOTO).

2. Sub-programação (ou modularização).

À medida que os programas vão se tornando maiores e mais complexos, é possível simplificar e melhorar a clareza dividindo o programa em partes menores, chamadas subprogramas.

Um subprograma, é um nome dado a um trecho de um programa mais complexo e que, em geral, encerra em si próprio um pedaço da solução de um problema maior (o programa a que ele está subordinado). São sinônimos usados na engenharia de software para o conceito de subprograma: procedimento, função, módulo (estrutura modular), métodos (orientação a objetos) e subrotina.

Na programação estruturada o "método dos refinamentos sucessivos" é uma "sistemática" de abordagem útil no projeto detalhado e na implementação de softwares. Partindo-se de um dado problema, para qual se deseja encontrar um programa de solução, deve-se procurar subdividi-lo em problemas menores e consequentemente de solução mais simples (dividir para conquistar). 

Alguns destes problemas menores (subproblemas) terão solução imediata (na forma de um subprograma) e outros não. Os subproblemas para os quais não for possível encontrar uma solução direta devem ser novamente subdivididos. Assim, o processo é repetido até que se consiga encontrar um subprograma para solucionar cada um dos subproblemas definidos.

Então, o programa de solução do problema original será composto pela justaposição dos subprogramas usados para solucionar cada um dos subproblemas em que o problema original foi decomposto.

Com a subdivisão de programas complexos algumas vantagens são conquistadas: 

&nbsp; &nbsp; ° (a) cada parte menor tem um código mais simples; 

&nbsp; &nbsp; ° (b) facilita o entendimento uma vez que os subprogramas podem ser analisados como partes independentes (legibilidade); 

&nbsp; &nbsp; ° (c) códigos menores são mais facilmente modificáveis para satisfazer novos requisitos do usuário e para correção de erros (manutenibilidade); 

&nbsp; &nbsp; ° (d) simplificação da documentação de sistemas; 

&nbsp; &nbsp; ° (e) desenvolvimento de software por equipes de programadores;

&nbsp; &nbsp; ° (f) reutilização de subprogramas através de bibliotecas de subprogramas, na linguagem C, sob a forma dos arquivos de cabeçalhos (.h)

A principal questão é a "reutilização de software" objetivando a economia de tempo e trabalho (benefícios técnicos que trazem vantagens financeiras). 

Um conjunto de subprogramas destinado a solucionar uma série de tarefas bastante corriqueiras é desenvolvido e vai sendo aumentado com o passar do tempo, com o acréscimo de novos subprogramas. A este conjunto dá-se o nome de biblioteca. No desenvolvimento de novos sistemas, procura-se ao máximo basear sua concepção em subprogramas já existentes na biblioteca, de modo que a quantidade de software realmente novo que deve ser desenvolvido é minimizada.

3. Tipos Abstratos de Dados.

Segundo o _Prof. Nivio Ziviani_, um Tipo Abstrato de Dados (TAD) pode ser visto como um modelo matemático, acompanhado das operações definidas sobre o modelo. O conjunto dos inteiros acompanhado das operações de adição, subtração e multiplicação forma um exemplo de um TAD.

Ainda segundo Ziviani, os TAD podem ser considerados generalizações de tipos primitivos de dados, da mesma forma que procedimentos são generalizações de operações primitivas tais como adição, subtração e multiplicação. 

Assim como um procedimento é usado para encapsular partes de um programa, o tipo abstrato de dados pode ser usado para encapsular tipos de dados.

Neste caso a definição do tipo de dados e todas as operações definidas sobre ele podem ser localizadas em uma única seção do programa (na Linguagem C, por exemplo, em um arquivo de cabeçalhos).

Em resumo as principais características da **Programação Estruturada** são:

&nbsp; &nbsp; ° decomposição gradativa dos programas ao nível fundamental (método dos refinamentos sucessivos, desenvolvimento top-down).

&nbsp; &nbsp; ° tipo abstrato de dados = modelo matemático + operações.

&nbsp; &nbsp; ° programação orientada a procedimentos: subprogramas => blocos estruturados de códigos (procedimentos, funções ou módulos) que funcionam da seguinte forma:

1. a comunicação entre os blocos se faz utilizando variáveis globais e pela passagem de dados através de parâmetros; 
 
2. os dados são processados nos blocos e migram de um bloco para outro, como mostra a figura abaixo, através de variáveis globais, parâmetros passados por referência e expressão retornada pela função (através do comando return na linguagem C); 

3. a execução de um programa é caracterizada pelo acionamento de um bloco de código. 

`OBS.: a utilização de variáveis globais não constitui uma boa prática de programação (escopo muito grande).`

![img01-TAD](https://arquivo.devmedia.com.br/artigos/Omero/ProgramacaoEstruturada/ProgramacaoEstruturada1.jpg)
