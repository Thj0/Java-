# Operadores 

Símbolos especiais que tem um significado próprio para a linguagem e estão associados a determinadas operações.

Geralmente as primeiras palavras que ouvimos em um curso de programação são: um programa é um conjunto de instruções lógicas que quando executadas, produzem algum resultado. Com isso em mente, ao começar a criar as primeiras linhas de código, logo notará que é comum receber dados do usuário, prover alguma lógica para processá-los e então apresentar o resultado desse processamento.

Então basicamente a proposta dos operadores são, realizar essas operações com a finalidade de um determinado resultado.

| Operador | Comparação  |
| -------- | ----------- |
| ==       | Igual       |
| !=       | Diferente   |
| <        | Menor       |
| >        | Maior       |
| <=       | Menor igual |
| >=       | Maior igual |



____

## Classificação dos Operadores

### Atribuição 

Representado pelo símbolo de igualdade =.

O operador de atribuição é utilizado para definir o valor inicial ou sobescrever o valor de uma variável. Em Java definimos um tipo, nome e opcionalmente atribuímos um valor à variável através do operador de atribuição. 

Por exemplo:

1. //classe Operadores.java
2. String nome = "Jhonata";
3. int idade = 22;
4. double peso = 68.5;
5. char sexo = 'M';
6. boolean doadorOrgao = false;
7. Date dataNascimento = new Date( );



_____

### Aritméticos 

O operador aritmético é utilizado para realizar operações matemáticas entre valores numéricos, podendo se tornar ou não uma expressão mais complexa.

Os operadores aritméticos são **+** (adição), **-** (subtração), ***** (multiplicação) e **/** (divisão).



1. //classe Operadores.java
2. double soma = 10.5 + 15.7; - //Um operador de atribuição com um aritmético, que é responsável por realizar uma soma. 
3. int subtração = 113 - 25; - //Um operador de atribuição com um aritmético, que é responsável por realizar uma subtração.
4. int multiplicação = 20 * 7; - //Um operador de atribuição com um aritmético, que é responsável por realizar uma multiplicação.
5. int divisao = 15 / 3; - //Um operador de atribuição com um aritmético, que é responsável por realizar uma divisão.
6. int modulo = 18 % 3; - //Um operador de atribuição com um aritmético, que é responsável por realizar um módulo.
7. double resultado = (10 * 7) + (20 / 4); 

_____



:exclamation: IMPORTANTE! O operador de adição (+), quando utilizado em do tipo texto, realizará a "concatenação de textos".



1. //classe Operadores.java
2. String nomeCompleto = "LINGUAGEM" + "JAVA";
3. 

4. //Qual o resultado das expressões abaixo?
5. String concatenação ="?";

6. 
7. concatenação = 1+1+1+"1"; // Enquanto o valor for numérico, a operação está servindo ou funcionando como soma, depois que o compilador percebeu que contém um texto ele concatena. 

Resultado - 31

8. 
9. concatenação = 1+"1"+1+1; // Depois que o compilador identifica uma concatenação na operação, ele não consegue mais realizar operações matemáticas. Ele entende que a partir dali, vai usar a concatenação.

Resultado - 1111

10. 
11. concatenação = 1+"1"+1+"1"; // Da mesma forma da operação passada, após a ocorrência detectada, ele deixa de fazer operações matemáticas e somente concatena.

Resultado - 1111

12. 
13. concatenação = "1"+1+1+1; // Após a ocorrência detectada, ele deixa de fazer operações matemáticas e somente concatena.

Resultado - 1111

14. concatenação = "1"+(1+1+1); // Primeiro é realizado a soma das evidências, daí ele guarda o resultado e depois concatena com o texto.

Resultado - 13



_____

