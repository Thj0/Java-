## Documentação.


Uma das maiores características da linguagem Java é que desde suas primeiras versões tínhamos em nossas mãos uma documentação rica e detalhada dos recursos da linguagem.

Conforme o site oficial, podemos compreender e explorar todos os recursos organizados por pacotes e classes bem específicas sem nem mesmo escrever uma linha de código.

Hoje costuma-se afirmar que para se tornar um desenvolvedor nível avançado, é um requisito imprescindível adquirir a habilidade de compreender a documentação oficial da linguagem e dos frameworks que são incorporados nos projetos atuais.

A documentação é composta por exemplos, detalhamentos, versões, formas de método, construtores e os atributos das classes que são disponibilizadas pela linguagem. 

[String](https://docs.oracle.com/javase/8/docs/api/java/lang/String.html)


___
## Tags 

Mas e quais informações que obtemos através de classes documentadas na linguagem? Java Documentation é composto por tags que representam dados relevantes para a compreensão da proposta de uma classe e os conjuntos de seus métodos e atributos conforme a tabela abaixo:


| Tag      | Descrição                                               |
| -------- | ------------------------------------------------------- |
| @autor   | Autor / Criador.                                        |
| @version | Versão do recurso disponibilizado.                      |
| @since   | Versão / Data de início da disponibilização do recurso. |
| @param   | Descrição dos parâmetros dos métodos.                   |
| @return  | Definição do tipo de retorno de um método.              |
| @throws  | Se o método lança alguma exceção.                       |

Abaixo iremos ilustrar classe Calculadora com um exemplo de documentação destacando as **tags** mais utilizadas.

```
/*
<h1>Calculadora</h1>
A Calculadora realiza operações matemáticas entre números 
<p>
<b>Note:</b> Leia atentamente a documentação desta classe para desfrutar dos recursos oferecidos pelo autor.

@autor Gleyson Sampaio
@version 1.0
@since 01/01/2022
*/

public class Calculadora {
	/**
	* Este método é utilizado para somar dois números inteiros.
	* @param numeroUm este é o primeiro parâmetro do método.
	* @param numeroDois este é o segundo parâmetro do método.
	* @return int o resultado deste método é a soma dos dois números.
	*/
	  
	  public int somar(int numeroUm, int numeroDois) {
		  return numeroUm + numeroDois ;
	  }

}
```


____
## Tipos de comentários 

One Line;

// Prazer, sou somente um comentário de uma linha.

___
Mult Line;

/.* Olá,
sou um comentário 
que posso ser mais detalhado 
quando necessário.
*/

___
Documentation

/**
*Estas duas estrelinhas acima
*é para identificar que você
*pretende elaborar um comentário
*à nível documentação.
*Muito mídia!
*/

___

*Um comentário não possui a finalidade de amenizar um algoritmo não estruturado conforme as convenções da linguagem.*

____

# Javadoc 

**Javadoc** é um gerador de documentação criado pela [Sun Microsystems](https://en.wikipedia.org/wiki/Sun_Microsystems) para documentar a [API](https://aws.amazon.com/pt/what-is/api/)dos programas em [Java](https://www.java.com/pt-BR/), a partir do [código-fonte]. O resultado é expresso em [HTML]. É constituído, basicamente, por algumas marcações muito simples inseridas nos comentários do programa.


Criando nossa documentação no formato HTML para disponibilizar via Web.

1. //No terminal eu executei o comando:

javadoc -encoding UTF-8 -docencoding ISO-8859-1 -d ..\Docs src\*.java
