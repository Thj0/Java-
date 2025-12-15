# Tipos e Variáveis 



## Tipos de dados 

No Java, existem algumas palavras reservadas para a representação dos tipos de dados básicos que precisam ser manipulados para a construção de programas. Estes tipos de dados são conhecidos como tipos primitivos (Primitive Types).

:grey_exclamation:**Os oito tipos primitivos em Java são:**

**int**, **byte**, **short**, **long**, **float**, **double**, **boolean** e **char** - esses tipos não são considerados objetos, e portanto representam valores brutos. Eles são armazenados diretamente na pilha de memória. (Memory stack)

____

**Tabela de Tipos Primitivos e seus valores:**

| Tipos | Memória | Valor mínimo                | Valor Máximo              |
| ----- | ------- | --------------------------- | ------------------------- |
| byte  | 1 byte  | - 128                       | 127                       |
| short | 2 bytes | - 32.768                    | 32.767                    |
| int   | 4 bytes | -2.147.483.648              | 2.147.483.647             |
| long  | 8 bytes | - 9.223.372.036.854.775.808 | 9.223.372.036.854.775.807 |

_____

**Os tipos primitivos que podem conter partes fracionárias, podem ser representados por dois tipos: **

| Tipos  | Memória | Mínimo          | Máximo       |
| ------ | ------- | --------------- | ------------ |
| float  | 4 bytes | - 3,402E + 38   | 3,4028E + 38 |
| double | 8 bytes | - 1,7976E + 308 | 17976E + 309 |

Apesar de o tipo **float** ocupar metade da memória consumida do que um tipo double, ele é menos utilizado. Ele sofre de uma limitação que compromete seu uso em determinadas situações; somente mantém uma precisão decimal entre 6 e 7 dígitos.

Atualmente, com os computadores modernos, se tornou desnecessário utilizar os tipos **short** e **byte**, pois não precisamos nos preocupar tanto assim com o espaço de memória reduzido.

Da mesma forma, dificilmente utilizaremos o tipo long, pois não é tão comum trabalharmos com valores tão grandes.

Portanto, para representar números, na grande maioria das vezes utilizamos o tipo **int** para representar números inteiros ou **double** para representar  números fracionados.

_____



:exclamation: O ponto mais relevante em compreender a definição dos tipos de dados é o momento da definição do tipo para uma variável. ***Qual tipo de dados eu utilizaria para determinar a idade de uma pessoa ou salário de um funcionário?***



____

## Declaração de Variáveis 

Variável é uma identificação de um espaço em memória utilizado pelo nosso programa. Segundo as convenções em linguagem de programação, toda variável é composta por: tipo de dados + identificação + valor atribuído.

A estrutura padrão para se declarar uma variável sempre é: 

'<Tipo>  <nomeVariavel>  <atribuicaoDeValorOpcional>'

Exemplo: 

1. int idade; //Tipo "int", nome "idade", com nenhum valor atribuído.
2. int anoFabricacao = 2021; //Tipo "int", nome "anoFabricacao", com valor atribuído "2021"
3. double salarioMinimo = 2.500; //Tipo "double", nome "salarioMinimo", com valor atribuído "2.500"



:exclamation:Existe algumas peculiaridades a trabalhar com alguns tipos específicos. Observe no exemplo abaixo:

1. public class TipoDados {
2. ​               public static void main (String[ ] args) {
3. ​                              byte idade = 123;
4. ​                              short ano = 2021;
5. ​                              int cep = 21070333; // se começar com zero, talvez tenha que ser outro tipo.
6. ​                              long cpf = 21397345678L; // se começar com zero, talvez tenha que ser outro tipo.
7. ​                              float pi = 3.14F;
8. ​                              double salario = 1275.33; 
9. ​                 }
10. }

____



:no_mobile_phones: Observe que o tipo **long** precisa terminar com L, e o tipo **float** com F. Em alguns cenários do dia a dia, podem estimular uma alteração de tipos de dados convencional.



Muitas das vezes criamos uma variável, definimos um valor correspondente, manipulamos esta variável e temos consciência de seu valor na aplicação. Porém, temos que ter cuidado!

____

:exclamation:Java é fortemente "tipado"

____



Veremos no cenário abaixo: 



1. // TiposEVariaveis.java
2. 

3. short numeroCurto = 1
4. int numeroNormal = numeroCurto;
5. short numeroCurto2 = numeroNormal;

_____

