# Anatomia das classes - 1º

***Uma classe bem estruturada não quer guerra com ninguém.***

____



A escrita de códigos de um programa é feito através da composição de palavras pré-definidas pela linguagem com as expressões que utilizamos para determinar o nome dos nosso arquivos, classes, atributos e métodos.

É muito comum mesclarmos expressões no idioma americano com o nosso vocabulário. Existe projetos que recomendam que toda a implementação do seu programa seja escrita na língua inglesa.





public class MinhaClass {

​         // Seu código aqui 

}



Dentro da minha classe ela pode ter várias composições, desde códigos, métodos, variáveis e expressões.

Por padrão, grande parte iniciarão com a expressão '**public class**', e o nome iterativo, intuitivo da minha classe. 

***Por exemplo:***

Ao criar uma classe de operações matemáticas, provavelmente esse classe iria ser chamada de 'calculadora' e não "MinhaClasse", e assim sucessivamente.

**Então é necessária a preocupação na distribuição de uma nomenclatura coerente.**

___

# Regra fundamental

- Letras maiúsculas.

É uma convenção de todos os arquivos que gerarmos, eles sempre começarão com a letra Maiúscula juntamente a cada palavra complementar, que também deve começar com a letra Maiúscula. 

**Então por padrão, todas as classes, precisarão ter a primeira letra como Maiúscula.**



____



Se a minha classe é executável, se é capaz de realizar uma inicialização do projeto ou de forma independente. 

Essa classe precisa de um método especial, ela precisa conter um método principal.

E esse método é chamado de **main**, que precisa seguir um padrão. 



public class MinhaClasse {

​        public static void main (String [ ]) args) { 

​                  System.out.print ( s );

​        }

}

O método main, tem uma característica única na sua representação de inicialização. O do exemplo usado foi o **'public static void'**.

E esse método, como já dito, espera um parâmetro especial. 

Dentro dos parênteses, no exemplo foi usado o parâmetro chamado de "**String**". E após, se abre os **colchetes [ ]**.

E daí a gente define esse parâmetro como **array**, a expressão usada para representar um array é "**args**".



Após isso dentro do corpo desse novo método, criaremos outra classe, chamada de "System", essa classe System é uma classe do sistema. Ela tem inúmeras operações de input e output, dentro da minha aplicação.

Na mesma linha determinamos a operação do sistema, "out" de output, e depois o método "print", junto de um parâmetro que se encontra dentro dos colchetes, o parâmetro de texto.



____

### Sobre JAVA.

Toda classe precisa existir dentro do 'src', como diretório do projeto. 

O nome, seja composto ou não, precisa iniciar com letras Maiúsculas.

E depois disso, é gerado para nós um bloco geral de código no qual a gente começa a desenvolver incluindo métodos, e operações internas.

____





