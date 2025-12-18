# Anatomia das classes - 3º



### Declarando variáveis e métodos 

Como identificar entre declaração de variáveis e métodos em nosso programa? Existe uma estrutura comum para ambas as finalidades, exemplo:

- Declarar uma variável em Java segue a seguinte estrutura: 



1. // Estrutura
2. .
3. Tipo NomeBemDefinido =  Atribuição ( opcional em alguns casos)
4. .
5. // Exemplo



7. int idade = 23;
8. double altura = 1.62;
9. Dog spike; //observe que aqui a variável spike não tem valor 

____

- Declarar métodos em Java segue uma estrutura bem simples: 

1. // Estrutura
2. .
3. TipoRetorno NomeObjetivoNoInfinitivo Parametro(s) - Os parâmetros podem ser opcional. - Alguns métodos podem exigir parâmetros, outros não. 

4. 

5. // Exemplo 

6. 

7. **int** somar (**int** numeroUm, **int** numero2)

8. 
9. String formatarCep (**long** cep)

____

:exclamation:Todos os métodos em Java costuma ser aplicado no infinitivo.

Ex: String -  somar, processar, incluir, formatar, calcular, adicionar.

Sempre no infinitivo.

____

- Agora um pequeno exemplo em código, de declaração de método:



public static void main(String [] args) {

​    

​    String nome = "Jhonata";

​    String  sobrenome = "Andrade";

​    String nomeCompleto = nomeCompleto (nome, sobrenome);

​    System.out.println(nomeCompleto);

  }



  public static String nomeCompleto(String nome, String sobrenome) {

​     return "Resultado do método: " + nome.concat(" ").concat(sobrenome);

  }

____



- Nesse exemplo acima criamos um método, sabendo que ele tem um tipo de retorno, e que esse tipo de retorno pode ser qualquer valor. Se quisermos que ele retorne um método inteiro, uma data, ou qualquer outra informação, eu só preciso dizer no início. Depois digo o nome compatível com a proposta, e se ele tiver parâmetros é só passar entre os parênteses informando o tipo, e após isso se tiver mais de um parâmetro é só separa-lo por ","(vírgula).

____

