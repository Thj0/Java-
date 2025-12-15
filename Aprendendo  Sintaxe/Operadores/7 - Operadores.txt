# Lógicos 

Os operadores lógicos representam o recurso que nos permite criar expressões lógicas maiores a partir da junção de duas ou mais expressões.



- **&&** Operador Lógico - "**E**"
- **||** Operador Lógico - "**OU**"

____

```java
//OPERADORES.java
boolean condicao1=true;

boolean condicao2=false;

/*Aqui estamos utilziando o operador lógico E para fazer a união das expressões 
É como se estivesse escrito:
  "Se Condicao1 e Condicao2 forem verdadeira, executar código"
  
```

Quando queremos verificar se as duas condições precisam ser verdadeiras, para me dar um ponto de execução ou um determinado resultado;



Usamos:

```java
boolean condicao1 = true;

boolean condicao2 = false;


if (condicao1 && condicao2){
	System.out.println("as duas condições são verdadeiras")
}

```

Porém percebemos que as condições não são iguais, logo não são verdadeiras. E com isso a mensagem não será executada.

____

Para confirmação;

```java
if (condicao1 && condicao2){
	System.out.println("as duas condições são verdadeiras")
}

System.out.println("fim")
```

Confirmando nossas evidências colocamos uma outra mensagem que vai ser executada.



Dessa forma, é fato de que a primeira mensagem solicitada não será executada, imprimindo somente "fim" no final.

____



```java
if (condicao1 || condicao2){
	System.out.println("uma das condições é verdadeira")
}

System.out.println("fim")
```

Mas em contrapartida com outra expressão lógica, determina-se que:



se a condicao1 OU a condicao2 é verdadeira.



**Logo o resultado será**:

'uma das condições é verdadeira'

fim.



Pois atende ao que estamos solicitando.

_____

**SE AS DUAS CONDIÇÕES FOREM VERDADEIRAS**: 

```java
boolean condicao1 = true;

boolean condicao2 = true;

    if (condicao1 && condicao2){
         System.out.println("as duas condições são verdadeiras");

    }

    if (condicao1 || condicao2){
         System.out.println("uma das condições é verdadeira");
    }
```

A 1° condição é verdadeira, então o resultado é:

'as duas condições são verdadeiras'



A 2° condição também é verdadeira, logo o resultado é: 

'uma das condições é verdadeira'



e por fim.

Obviamente será exibida as duas mensagens.

____

***RESUMO RÁPIDO*** 

- O **&&** "E" ele valida as duas condições.
- O **||** "OU" verifica se alguma das condições é verdadeira.

Essa é a proposta dos operadores lógicos.

____

***Nem sempre precisamos ter uma expressão booleana previamente definida; podemos criar uma expressão relacional que, ao ser avaliada como verdadeira, retornará o resultado esperado.***



Exemplo:

```java
if (condicao1 && 7 > 4 ){
         System.out.println("as duas condições são verdadeiras");
}
```

"se a condicao1 E 7 for MAIOR QUE  4"



Eu também tenho um valor booleano true.

Esses tipos de expressões relacionais. também representam uma declaração booleana nos nossos algoritmos.



______

Então percebemos que expressões lógicas comtemplam valores booleanos ou expressões relacionais, que representam uma valoração/atribuição booleana.