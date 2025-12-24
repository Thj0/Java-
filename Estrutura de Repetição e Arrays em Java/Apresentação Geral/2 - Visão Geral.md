Estruturas de Repetição e Arrays

____
### Estrutura de Repetição 

O poder dos computadores está na sua habilidade para repetir uma operação ou uma série de operações várias vezes.

Cada repetição é chamada de laço (loop), é um dos conceitos básicos da programação estruturada.

**Uma estrutura de repetição permite que uma sequência de comandos seja executada repetidamente, caso determinadas condições sejam satisfeitas.**

Essas condições são representadas por expressões lógicas.

___
As estruturas de repetição podem ser classificadas em: 
 - Repetição com teste no início (while)
 - Repetição com teste no final (do-while)
 -  Repetição contada (for)

O comando brak é utilizado para terminar de forma abrupta uma repetição. 

Quando o comando continue é executado, os comandos restantes da repetição são ignorados e o programa volta a testar novamente ou não.

____

_**while_

![[Pasted image 20251223114636.png]]



Fluxograma feito para explicar de forma conceitual.

While (enquanto).

No exemplo acima como vemos, ao dar ínicio ao programa passando pela expressão e chegando na sentença enquanto(while) o valor for 1, repita o processo.

Porém caso a expressão seja 0, o programa não entra na sentença e encerra.

__

Falando sobre break, quando o programa executar e passar pela sentença, mas nela haver um break.

A sentença é interrompida abruptamente e encerra(fim). 
Não resultando em uma repetição(loop).

___
Sobre o continue, caso o programa passe pela sentença e nela tenha um continue, o programa ignora os comandos abaixo, não os executando e retorna a expressão.

Resultando em um loop(repetição).

____
_**do-while_

![[Pasted image 20251223120611.png]]


Já no do-while, a sentença é iniciada independente se o valor for true ou false.
Após a sentença, que temos a expressão.

Daí caso seja true, o comando é executado mais uma vez e cai novamente na expressão.

Porém se ao passar pela expressão e o valor for false, o laço encerra.

____

_**for_

![[Pasted image 20251223124036.png]]

Sobre o for, primeiro se inicializa o programa, depois passa por um teste.

Após esse teste, caso seja true executa a sentença que vai haver uma atualização.

No for é obrigatório ter essa atualização.
Após essa atualização o comando retorna pro teste, ocasionando em uma repetição(loop).

Caso o comando passe pelo teste e o valor for false, ele encerra o programa.

Essa atualização pode ser feita tanto no do-while, quanto no while.

_____
### OPERADORES DE INCREMENTO E DECREMENTO 

## Pré-fixados.


| Para:                                     | Use o atalho: | Forma original:                      |     |     | -   |
| ----------------------------------------- | ------------- | ------------------------------------ | --- | --- | --- |
| Somar uma unidade ao valor da variável    | ++numero;     | número = numero +1; (retorne numero) |     |     | +   |
|                                           |               |                                      |     |     | T   |
| Subtrair uma unidade do valor da variável | -- numero;    | numero = numero -1; (retorne numero) |     |     | -   |

No pré fixado, primeiro fazemos a soma e depois retornamos o numero.

De forma mais simples:
Primeiro altera o valor, depois usa(retorna) o novo valor.
___
## Pós-fixados.


| Para:                                                           | Use o atalho: | Forma original:                      |     |     | -   |
| --------------------------------------------------------------- | ------------- | ------------------------------------ | --- | --- | --- |
| Somar um, ao valor da variável, retornando o valor original.    | numero++;     | (retorne numero) numero = numero +1; |     |     | +   |
|                                                                 |               |                                      |     |     | H   |
| Subtrair um, do valor da variável, retornando o valor original. | numero--;     | (retorne numero) numero = numero -1; |     |     | -   |

Já no pós-fixado, primeiro retornamos o número e depois fazemos a soma 

De uma forma mais simples:
Primeiro usa (retorna) o valor atual, depois altera o valor.

___
### Observação importante!
Se não houver uso do valor no momento (ex: não está em  **println, if , atribuição etc.), não há diferença prática: 

```Java

numero++;
++numero;

```

Ambos fazem exatamente a mesma coisa nesse caso.


___
## OPERAÇÕES ARITMÉTICAS


| Para:                                    | Use o atalho:  | Forma original:      |
| ---------------------------------------- | -------------- | -------------------- |
| Somar k unidades ao valor da variável    | numero + = k ; | numero = numero + k; |
| Subtrair k unidades do valor da variável | numero -= k ;  | numero = numero - k; |
| Multiplicar o valor da variável por k    | numero *= k ;  | numero = numero * k; |
| Dividir o valor da variável por k        | numero /= k ;  | numero = numero / k; |

____

## ARRAYS

Um Array é um objeto utilizado para armazenar sequencialmente dados do mesmo tipo.

Permanecem com o mesmo tamanho depois de criados.

Array UNIDIMENSIONAL

![[Pasted image 20251223143504.png]]


( C ) é o nome da variável, e os números dentro dos colchetes [  ] são as posições. 
O índice é o que ta dentro do colchetes que no caso são as posições.

E cada posição guarda um valor aleatório.

____

Array MULTIDIMENSIONAL


![[Pasted image 20251223143546.png]]

Esse é um Array Multidimensional.

Porém o da imagem se trata de um bidimensional, porque como está sendo mostrado, contém somente linhas e colunas.


 O primeiro colchete guarda a posição da linha, 
 e o segundo colchete guarda a posição da coluna.

Como sabemos, o nome da variável é a letra ( a ) que está do lado de fora dos colchetes.


Exemplo:

|         | COLUNA 0        | COLUNA 1        | COLUNA 2        | COLUNA 3        |
| ------- | --------------- | --------------- | --------------- | --------------- |
| LINHA 0 | a [ 0 ] - [ 0 ] | a [ 0 ] - [ 1 ] | a [ 0 ]- [ 2 ]  | a [ 0 ] - [ 3 ] |
| LINHA 1 | a [ 1 ] - [ 0 ] | a [ 1 ] - [ 1 ] | a [ 1 ] - [ 2 ] | a [ 1 ] - [ 3 ] |
| LINHA 2 | a [ 2 ] - [ 0 ] | a [ 2 ] - [ 1 ] | a [ 2 ] - [ 2 ] | a [ 2 ] - [ 3 ] |
| LINHA 3 | a [ 3 ] - [ 0 ] | a [ 3 ] - [ 1 ] | a [ 3 ] - [ 2 ] | a [ 3 ] - [ 3 ] |

____