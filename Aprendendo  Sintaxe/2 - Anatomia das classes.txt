# Anatomia das classes - 2º



## Convenções de escrita

#### Padrão de nomenclatura 

Quando se trata de escrever código na linguagem Java, é recomendado seguir algumas convenções de escrita. Esses padrões estão expressos nos itens abaixo:

- **Arquivo .java:** Todo arquivo .java deve começar com letra MAIÚSCULA. Se for composta, a segunda palavra deve também ser maiúscula, exemplo:

Calculadora.java, CalculadoraCientifica.java

- **Nome da classe no arquivo:** A classe deve possuir o mesmo nome do arquivo.java, exemplo:



// arquivo CalculadoraCientifica.java



​       public class CalculadoraCientifica {



}



- **Nome de variável:** Toda variável deve ser escrita com letra minúscula, porém se a palavra for **composta**, a primeira letra da **segunda palavra** deverá ser MAIÚSCULA, exemplo: ano e anoFabricacao. O nome dessa prática para nomear variáveis dessa forma se chama de "camelCase".

Se tivermos uma variável com 3 palavras compostas, a partir da segunda a letra inicial dessas palavras tem que ser Maiúscula.



:exclamation:Existe uma regra adicional para variáveis quando na mesma queremos identificar que ela não sofrerá alteração de valor, exemplo: queremos determinar que uma variável de nome **BR** sempre representará **"Brasil"** e nunca mudará seu valor, logo, determinamos como escrita o código abaixo:

String BR = "Brasil"   - Variável camelCase

double PI = 3.14

int ESTADOS_BRASILEIRO = 27   - Variável upperCase

int ANO_2000 = 2000

____

- ***Variável camelCase*** - É uma convenção de nomenclatura em programação onde várias palavras são unidas em uma só, sem espaços, com a primeira letra de cada palavra (exceto a primeira, no caso do *lowerCamelCase*) em maiúscula.



- ***Variável upperCase*** -  É uma variável nomeada seguindo uma convenção de separação, que pode ser feita com o underline (_) ou outra forma, desde que o símbolo utilizado siga as regras de nomenclatura da linguagem.

⚠ Mas **não é qualquer símbolo**, por exemplo: `@`, `#`, `%`, `-` não são permitidos em nomes de variáveis.



- **PascalCase** - É uma convenção de escrita onde **cada palavra começa com letra maiúscula**, sem espaços e **sem underline**.

  

____



***final -*** Na linguagem Java, "final" tem um significado oculto porque ela é uma palavra reservada, É como se fosse um atalho para definir uma variável, como constante.

Um exemplo citado acima é o valor de PI, que nunca vai ser alterado. Ou seja, ao declarar a variável de letras Maiúsculas atribuida a 'final', ela se torna uma constante. 

E não pode mais ser alterada, resultando em um valor fixo.

- Caso eu queria especificar algo eu uso o "_" (underline)

Ex: int ANO_2000 = 2000



____



:heavy_exclamation_mark:Recomendação: Para declarar uma variável nós podemos utilizar caracteres, números e símbolos, porém devemos seguir algumas regras da linguagem.  

- Deve conter apenas letras, _ (underline), $ ou os números de 0 a 9.
- Deve obrigatoriamente se iniciar por uma letra (preferencialmente), _ ou $, jamais com número.
- Deve iniciar com uma letra minúscula (boa prática - ver abaixo).
- Não pode conter espaços.
- Não podemos usar palavras-chave da linguagem.
- O nome deve ser único dentro de um escopo. 



1. // Declarações inválidas de variáveis



3. int numero**&**um = 1;   //Os únicos símbolos permitidos são _ e $.
4. int 1numero = 1;    //Uma variável não pode começar com números
5. int numero um = 1;     //Não pode ter espaço no nome da variável.
6. int long = 1;     //long faz parte das palavras reservadas da linguagem 
7. 

8. // Declaração válida de variáveis
9. int numero**$**um = 1;
10. int numero1 = 1;
11. int numeroum = 1;
12. int longo = 1;
13. 

____



