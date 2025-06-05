# Jogo de Xadrez

Este repositório contém o seguinte arquivo:

- Jogo de Xadrez

## Descrição

Atividade relacionada ao desafio **Super Trunfo**.

**O trabalho contido neste repositório integra o desenvolvimento do TCC.**

# Explicação 

## **Simulação de Movimentos de Peças de Xadrez em C (Jogo de Xadrez)**

Este código em C foi projetado para simular, de forma simplificada, os movimentos de algumas peças de xadrez: Torre, Bispo, Rainha e Cavalo. O desenvolvimento seguiu uma abordagem estruturada, focada em atender a requisitos específicos de demonstração de diferentes estruturas de controle e saídas de dados.

## Principais Etapas do Desenvolvimento

1.  **Definição de Requisitos e Constantes:**
    * Foram estabelecidos requisitos funcionais para cada peça, como o número de "casas" que cada uma deveria se mover e a direção. Esses números foram definidos como constantes (`#define`) no início do código para fácil visualização e modificação (ex: `MOVIMENTOS_TORRE`, `CAVALO_PASSOS_PARA_BAIXO`).
    * Requisitos não funcionais, como legibilidade, documentação e simplicidade (adequada para um nível básico/intermediário), também guiaram o desenvolvimento, como indicado nos comentários do código.

2.  **Estrutura Modular com Funções:**
    * Para cada peça, uma função específica de simulação de movimento foi criada (`simularMovimentoTorre`, `simularMovimentoBispo`, `simularMovimentoRainha`, `simularMovimentoCavalo`). Isso torna o código organizado e fácil de entender.
    * Os protótipos dessas funções foram declarados no início do arquivo.

3.  **Implementação dos Movimentos das Peças:**
    * **Torre, Bispo e Rainha:** Para as três primeiras peças, foi seguido o requisito de utilizar uma estrutura de repetição diferente para cada uma:
        * `simularMovimentoTorre()`: Utiliza um loop `for` para simular o movimento da torre.
        * `simularMovimentoBispo()`: Utiliza um loop `while` para o movimento do bispo.
        * `simularMovimentoRainha()`: Utiliza um loop `do-while` para o movimento da rainha, com uma verificação para garantir que o loop só execute se o número de movimentos for maior que zero.
    * **Cavalo:** A simulação do movimento do cavalo (`simularMovimentoCavalo()`) foi implementada para seguir um padrão em "L" específico (duas casas para baixo, uma para a esquerda). Conforme um requisito implícito pela estrutura do código, utilizou-se loops aninhados: um loop `for` externo (que executa apenas uma vez para representar o único movimento em "L" solicitado) contendo um loop `for` para os movimentos verticais ("Baixo") e um loop `while` para o movimento horizontal ("Esquerda").

4.  **Função Principal (`main`):**
    * A função `main` orquestra a simulação, chamando cada uma das funções de movimento em sequência.
    * Inclui mensagens de `printf` para indicar o início e o fim da simulação, e para separar a saída de cada peça, incluindo uma linha em branco específica antes do movimento do cavalo, conforme solicitado.

5.  **Documentação:**
    * O código foi extensivamente comentado para explicar a lógica de cada parte, os requisitos funcionais e não funcionais atendidos, e as simplificações adotadas. Isso inclui comentários de cabeçalho para funções (estilo Doxygen) e explicações inline.

## Resumo

Em resumo, o código foi desenvolvido com um foco didático, demonstrando o uso de diferentes estruturas de loop (`for`, `while`, `do-while`) e loops aninhados, dentro de um contexto simples de simulação de movimentos de peças de xadrez. A clareza, a organização em funções e a documentação foram aspectos importantes considerados durante sua criação.
