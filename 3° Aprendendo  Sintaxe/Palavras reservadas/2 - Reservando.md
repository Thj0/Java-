# Palavras reservadas 

Palavras reservadas são identificadores de uma linguagem que já possuem uma finalidade específica, portanto não podem ser utilizados para nomear variáveis, classes , métodos ou atributos.

A linguagem Java possui 52 palavras reservadas. Todas essas palavras são classificadas em grupos e escritas com letra minúscula, sendo identificadas com uma cor especial pela maioria das IDE's. Abaixo temos a lista de palavras agrupadas por suas finalidades.

____



### Palavras Reservadas em Java

|          |          |            |           |              |
| -------- | -------- | ---------- | --------- | ------------ |
| abstract | continue | goto       | package   | synchronized |
| assert   | default  | if         | private   | this         |
| boolean  | do       | implements | protected | throw        |
| break    | double   | import     | public    | throws       |
| byte     | else     | instanceof | return    | transient    |
| case     | extends  | int        | short     | try          |
| catch    | final    | interface  | static    | void         |
| char     | finally  | long       | strictfp  | volatil      |
| class    | float    | native     | super     | while        |
| const    | for      | new        | switch    |              |

____



***Controles de pacotes***

**import**: importar pacotes ou classes para dentro do código.

**package**: especifica a que pacote todas as classes de um arquivo pertencem.



____

***Modificadores de acesso***

**public**: acesso de qualquer classe.

**private**: acesso apenas dentro da classe.

**protected**: acesso por classes no mesmo pacote e subclasses.



____

***Primitivos***

**boolean**: um valor indicando verdadeiro ou falso.

**byte**: um inteiro de 8 bits (signed).

**char**: um character unicode (16-bit unsigned)

**double**: um número de ponto flutuante de 64 bits (signed).

**float**: número de ponto flutuante de 32 bits (signed).

**int**: um inteiro de 32 bits (signed).

**long**: um inteiro de 64 bits (signed).

**short**: um inteiro de 32 bits (signed).

**void** indica que o método não tem retorno **de valor**.



____

***Modificadores de classes, variáveis ou métodos***

**abstract**: classe que não pode ser instanciada ou método que precisa ser implementado por uma subclasse não abstrata.

**class**: especifica uma classe.

**extends**: indica uma superclasse que a subclasse está estendendo 

**final**: impossibilita que uma classe seja estendida, que um método seja sobrescrito ou que uma variável seja reinicializada.

**implements**: indica as interfaces que uma classe irá implementar.

**interface**: especifica uma interface.

**native**: indica que um método está escrito em uma linguagem dependente de plataforma, como o C

**new**: instancia um novo objeto, chamando seu construtor.

**static**: faz um método ou variável pertencer à classe ao invés de às instâncias.

**strictfp**: usado em frente a um método ou classe para indicar que os números de ponto flutuante seguirão as regras de ponto flutuante em todas as expressões.

**synchronized** indica que um método só pode ser acessado por uma thread de cada vez.

**transient**: impede a serialização de campos.

**volatile**: indica que uma variável pode ser alterada durante o uso de threads.



____

***Controle de fluxo dentro de um bloco de código***

**assert**: verifica uma condição durante a execução (debug).

**break**: sai do bloco de código em que ele está.

**case**: executa um bloco de código dependendo do teste do switch.

**catch**: captura e trata uma exceção.

**continue**: pula a execução do código que viria após essa linha e vai para próxima passagem do loop.

**default**: executa quando nenhum **case** é atendido.

**do**: laço de repetição com teste no final.

**finally**: bloco que sempre será executado após **try/catch**.

**for**: laço de repetição com controle de inicialização, condição e incremento.

**else**: executa um bloco caso a condição do **if** seja falsa.

**if**: executa um bloco se a condição for verdadeira.

**return**: retorna um valor (ou encerra) um método.

**switch**: seleciona a execução com base em um valor.

**throw**: lança explicitamente uma exceção.

**throws**: declara exceções que um método pode lançar.

**while**: laço de repetição com teste no início.



____

***Orientação a objetos / uso interno***

**this**: referência ao objeto atual.

**super**: referência à superclasse.

**instanceof**: testa se um objeto pertence a um tipo/classe.



____

***Estruturas de tipos modernas***

**enum**: define um conjunto fixo de constantes.

**non-sealed**: remove a restrição de herança de uma classe selada.

**permits**: define quais classes são permitidas em uma classe **sealed**.

**record**: classe imutável usada para transporte de dados.

**sealed** restringe quais classes podem estender outra.



____

***Palavras reservadas do sistema de módulos (Java9+)***

**exports**: torna um pacote acessível a outros módulos.

**module**: define um módulo.

**opens**: permite reflexão em um pacote.

**provides**: fornece uma implementação de serviço.

**requires**: declara dependência de outro módulo.

**to**: especifica módulos de destino (**exports / opens**).

**transitive**: repassa dependências automaticamente.

**uses**: declara uso de um serviço.



____

***Palavras reservadas especiais***

**const**: reservada, não utilizada.

**goto**: reservada, não utilizada. 

**var**: inferência de tipo local (contextual).

**yield**: retornar valor em expressões **switch**.



____

### Palavras "opostas"

Assim como nas classificações gramaticais da língua português, existem algumas palavras que são completamente opostas (antônimas) na linguagem Java conforme tabela abaixo:

opostas = substituição







____

