# Ternário 

O Operador de Condição Ternária é uma forma resumida para definir uma condição e escolher por um dentre dois valores. Você deve pensar numa condição ternária como se fosse uma condição IF normal, porém de uma forma em que toda a sua estrutura estará escrita numa única linha.



o operador ternário é representado pelos símbolos  **?:**  utilizados na seguinte estrutura de sintaxe:

<Expressão Condicional>  **?** <Caso condição seja true> **:**  <Caso a condição seja false> 



Exemplos abaixo: 

// classe Operadores.java

int a, b;



a = 5;

b = 6;

 

/* Exemplo de condicional utilizando uma estrutura IF/ELSE */

if (a == b) {

​     resultado = "verdadeiro";

} else {

​     resultado = "falso";

}

System.out.println(resultado);



O resultado impresso é falso.

____

### Atribuindo condicional com operador ternário 

É possível abreviar a lógica acima utilizando o **operador ternário**.



Exemplo:



int a, b;



a = 5;

b = 6;



String resultado = a == b ? "verdadeiro" : "falso"; /* Se a for igual a b, atribui "verdadeiro",
   caso contrário, atribui "falso" */



System.out.println(resultado);



O resultado impresso é falso.

____

**Condição verdadeira**

Exemplo:



int a, b;



a = 6;

b = 6;



String resultado = a == b ? "verdadeiro" : "falso";  /* Se a for igual à b, imprima(?) "verdadeiro", senão( : ) "falso"; 

System.out.println(resultado);



O resultado impresso será verdadeiro.

____



📌 **Resumo rápido**:

- O operador ternário substitui **if/else** simples.
- Sempre retorna **um valor**.
- Deve ser usado quando a lógica for **curta e clara**.



____

**Lembrando!**

A primeira operação é de necessidade que seja booleana, sempre checar e analisar se a expressão retornará um valor de "true" ou "false".



Se o resultado é uma string, espera-se que os valores sejam strings.

Se o resultado for um inteiro(int), espera-se que o valor sela numérico.





os dois valores possíveis (`valor_se_true` e `valor_se_false`) **precisam ser do mesmo tipo ou compatíveis entre si**.



#### Exemplo correto:

```
String resultado = condicao ? "Sim" : "Não";
int resultado = condicao ? 1 : 0;
```

#### Exemplo incorreto:

```
int resultado = condicao ? 1 : "zero"; // ERRO
```



------

📌 **Resumo mental**:

- A condição → sempre booleana
- Os dois resultados → **mesmo tipo (ou tipos compatíveis)**
- O tipo da variável que recebe o resultado deve bater com os valores retornados