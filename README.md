# Graphs
Trabalho de Estrutura de Dados 2 - Implementação de um grafo em C e utilização do Algoritmo de Bellman-Ford de caminho mínimo.

DESCRIÇÃO DO TRABALHO

Objetivo

Desenvolver uma aplicação em linguagem C capaz de resolver um problema de otimização com base em algoritmos de grafos.


Descrição

O problema do caminho mínimo consiste em encontrar o caminho de menor custo que começa em um vértice o e termina em um vértice d. Uma vez definido tal problema, o presente trabalho consiste em criar um programa que suporte os seguintes comandos lidos a partir de um prompt na tela ou de um arquivo texto informado:


Comando Descrição

CV v - Cria um vértice com o identificador v

RV v - Remove o vértice identificado por v

CA a v1 v2 x - Cria uma aresta com o identificador a incidindo nos vértices de identificadores v1 e v2. O valor armazenado na aresta é um número inteiro especificado por x.

RA a - Remove a aresta identificada por a.

TA a x - Troca o valor armazenado na aresta de identificador a pelo valor x.

IG - Imprime o grafo na tela.

Para definir a forma que seu programa deve imprimir o grafo na tela, considere um grafo com n vértices, m arestas, identificadores de vértices v1, v2, ..., vn, identificadores de arestas a1, a2, ..., am com respectivos valores x1, x2, ..., xm.
Assuma ainda que ui e wi representam os identificadores dos vértices em que a aresta ai incide, sendo extraídos do conjunto {v1, ..., vn}. A saída do comando deve ser a seguinte:

Qtd de vértices: n

v1 v2 ... vn

Qtd de arestas: m

a1 u1 w1 x1

a2 u2 w2 x2

...

am um wm xm

Os identificadores de vértices devem ser impressos em ordem crescente: v1 < v2 < ... < vn

Os identificadores de arestas devem ser impressos em ordem crescente: a1 < a2 < ... < am

Os identificadores de vértices em que a aresta ai incide devem ser impressos em ordem crescente: ui < wi

CM v1 v2 Determina e imprime o caminho mínimo entre o vértice de identificador v1 e o vértice de identificador v2.

A saída do comando deve ser a seguinte:

Custo: c

Caminho: v1 ... vi vj ... v2

FM Termina a execução do seu programa. Todas as estruturas dinâmicas devem ser desalocadas e seu programa deve encerrar.

Além de suportar os comandos acima, o seu programa deve obrigatoriamente atender aos seguintes requisitos:

1. Os grafos devem ser montados sem considerar orientação nas arestas.

2. Toda a funcionalidade de consulta e manipulação do grafo (ex: inserções e remoções de vértices e arestas, consulta dos vizinhos de um vértice, etc) devem estar isoladas em um TAD (Tipo Abstrato de Dados) denominado Grafo.

3. A rotina de cálculo do caminho mínimo deve receber como parâmetros um Grafo montado e os identificadores dos vértices de origem e destino dentro do grafo.

Sua implementação deve ser feita somente através de chamadas às operações definidas no TAD Grafo. Não será permitido o uso de bibliotecas que forneçam as estruturas de dados prontas.
