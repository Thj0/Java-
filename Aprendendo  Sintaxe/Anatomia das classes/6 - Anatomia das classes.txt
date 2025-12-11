# Java Beans 



Umas das maiores dificuldades na programação é escrever algoritmos legíveis a níveis que seja compreendidos por todo seu time ou por você mesmo no futuro. Para isso a linguagem Java sugere, através de convenções, formas de escrita universal para nossas classes, atributos, métodos e pacotes.

____

***O que é?***

Java Beans é uma iniciativa conceitual da comunidade para que a gente possa ter uma estruturação de escrita. Não só identação, e tabulação, mas também de como expressamos as declarações das nossas variáveis, métodos, classes e etc.

____

***O que isso quer dizer?***

É que a gente precisa impor clareza nas nossas escritas. Na definição dos nomes dos nosso arquivos, das nossas variáveis, métodos e assim por diante.

____

***Como melhoras esses aspectos?***



**Variáveis**

Anteriormente já aprendemos algumas regras de declaração de variáveis, mas agora iremos conhecer algumas sugestões de nomenclatura:

- Uma variável deve ser clara, sem abreviações ou definição sem sentido;

- Uma variável é sempre no singular, **exceto quando se referir a um array ou coleção**.

- Defina um idioma único para suas variáveis.

  Se declarei a primeira variável em inglês, ou em qualquer outro idioma, tenho que definir todas em inglês, ou no respectivo idioma. 

____

**Não recomendado**

1. double salMedio = 1500.23     // variável abreviada
2. String emails = "aluno@escola.com"     // confuso
3. String myName = "JOSEPH" //  se o idioma é pt-BR, o valor tem que ser pt-BR.

____

**Recomendado**

1. double salarioMedio = 1500.23;
2. String email = "aluno@escola.com";
3. String [ ] emails = {"aluno@escola.com","professor@escola.com}
4. String meuNome = "JOSEPH"

____

**Métodos**

Os métodos deverão ser nomeados como verbos, através de uma mistura de letras minúsculas e maiúsculas. Em princípio todas as letras que compõem o nome devem ser mantidas em minúsculo, com exceção da primeira letra de cada palavra composta a partir da segunda palavra.

Exemplos sugeridos para numenclatura de métodos:

1. somar (int n1, int n2) { }
2. 

3. abrirConexao( ){ }
4. 

5. concluirProcessamento( ){ }
6. .

7. findById(int id){ } // Veremos muitos métodos em inglês pela nossa jornada.

8. 
9. calcularImprimir( ){ } // há algo de errado nesse, ele deveria ter uma única finalidade.

____

Essas convenções elas nos trazem um direcionamento melhor, uma interpretação mais abrangente. E também uma melhor distribuição da nossa lógica de negócio.