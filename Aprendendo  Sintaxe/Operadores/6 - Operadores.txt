# Relacionais 

Os operadores relacionais avaliam a relação entre duas variáveis ou expressões. Neste caso, mais precisamente, definem se o operando à esquerda é igual, diferente, menor, OU menor igual, maior OU maior igual ao da direita, retornando um valor boolano como resultado.



- **==** Quando desejamos verificar se uma variável é **IGUAL A** outra.
- **!==** Quando desejamos verificar se uma variável é **DIFERENTE** da outra.
- **>** Quando desejamos verificar se uma variável é **MAIOR QUE** a outra.
- **>=** Quando desejamos verificar se uma variável é **MAIOR OU IGUAL** a outra.
- **<** Quando desejamos verificar se uma variável é **MENOR QUE** a outra.
- **<=** Quando desejamos verificar se uma variável é **MENOR OU IGUAL** a outra.

____



**EXEMPLO - 1:**

```java
public static void main (String[] args){ 
	int numero1 = 1;
 	int numero2 = 2;
 

 		if (numero1 > numero2) {}
			System.out.println("Número 1 maior que número 2");
 
 		if (numero1 < numero2) {}
 			System.out.println("Número 1 menor que número 2");
}    
```



____

**EXEMPLO - 2:**

```java
PUblic static void main (String[] args) {
	int numero1 = 1;
    int numero2 = 2;

     boolean simNao = numero1 == numero2;

        if (numero1 < numero2){
            System.out.println("a nossa condição é verdadeira.");
        } else { 
            System.out.println("a nossa condição é falsa.");
        }    
    

        System.out.println("numeroUm é igual a numeroDois?" + simNao);

        simNao = numero1 != numero2;

        System.out.println("numeroUm é diferente de numeroDois?" + simNao);

        simNao = numero1 > numero2;

        System.out.println("numeroUm é maior que numeroDois?" + simNao);
}
```

Criamos a variável booleana para determinar uma condição dentro da aplicação, e consequentemente o resultado foi falso(false).

Replicamos a variável, e a atribuímos utilizando uma outra expressão para a mesma variável. E o resultado foi verdadeiro(true).

Novamente replicando com outra expressão, o resultado obtido foi falso(false).



**Essa proposta é utilizada bastante em validações**, e essas validações são utilizadas em **condições.**

Então, dependendo se a condição for verdadeira o fluxo será executado, do contrário nos mostraria outro comportamento.

Porém a ideia foi enfatizar a usabilidade dos operadores relacionais.



Na dinâmica apresentada pelo professor, foi dada a ênfase somente a um pequeno fluxo com o **if**, eu que resolvi arriscar utilizando o **else** na aplicação.

Porém a ideia foi enfatizar a usabilidade dos operadores relacionais.



Os operadores relacionais nos auxiliam em tomadas de decisão, e consequentemente realizam **fluxos** na nossa aplicação dependendo se a expressão for verdadeira(true).

____

**EXEMPLO - 3:**



```java
public static void main (String[] args) {
	String nomeUm = "Thjo";
    String nomeDois = ("Thjo");

    System.out.println(nomeUm == nomeDois);
}


```

Precisamos compreender que nem sempre falamos de números para as nossas comparações, Também comparamos, textos, objetos e etc...

Então quando falamos de textos ou objetos; Valores além de ser numérico.

Entendemos que existirão as nossas classes, Ex: String, funcionário, cliente. E queremos comparar se dois objetos são iguais.

Dado a devida ênfase nessa proposta, com as variáveis criadas, o resultado é true.

**Oque entendemos?**

Que conseguimos avaliar que é possível verificar conteúdos, as nossas **Strings**.

____

**EXEMPLO - 4:** 

```java
 public static void main (String[] args) {
     String nomeUm = "Thjo";
     String nomeDois =  new String("Thjo");

     System.out.println(nomeUm == nomeDois);
 }
```

O resultado é false.



Contendo uma pegadinha **new String("Thjo")**, criando um novo objeto o resultado é false, porque existem dois objetos.

Isso acontece porque existem 2 objetos **na memória**, quando falamos de números a linguagem Java tem uma compreensão, eles vão para espaços em memórias.

Quando falamos sobre objetos, esses valores são aplicados de uma outra estrutura.

Costuma-se usar o método **equals**(anObject). 

Esse método compara conteúdos, como temos 2 no exemplo  apresentado, ele checa se o conteúdo desses dois objetos são iguais.

____

**EXEMPLO - 5:**

```java
public static void main (String[] args) {
    String nomeUm = "Thjo";
    String nomeDois =  new String("Thjo");

    System.out.println(nomeUm.equals(nomeDois));
}
```

Como apresentado, utilizando **equals** para objetos, é a forma mais recomendada.



____

***Resumo rápido***

* Para números podemos utilizar os operadores relacionais.
* Mas quando se fala de objetos, utilizamos o método **equals** de comparação de conteúdo.