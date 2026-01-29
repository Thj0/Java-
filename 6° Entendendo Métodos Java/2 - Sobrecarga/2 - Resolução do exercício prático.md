
O exercício tem como objetivo criar um programa que calcula a área dos 3 quadriláteros notáveis, com foco em utilizar sobrecarga.

```java 

/* Clase de exemplo para o exercício da Aula 2 de métodos.*/

  

public class Quadrilatero {

    public static void area(double lado) { // Um double

  

        System.out.println("Área do quadrado: " + lado * lado);

    }

  

    public static void area(double lado1, double lado2) { // Dois double

  

        System.out.println("Área do retângulo: " + lado1 * lado2);

    }

  

    public static void area(double baseMaior, double baseMenor, double altura){ // Três double

  

        System.out.println("Área do trapézio: " + ((baseMaior + baseMenor)*altura) / 2);

    }

  

}
```

À princípio essa foi a aplicação criada.

junto a classe main: 

```java
public class Main {

  

    public static void main(String[] args) {

        // Quadrilátero

        System.out.println("Exeercício quadrilátero");

  

        Quadrilatero.area(3);

        Quadrilatero.area(5d, 5d);

        Quadrilatero.area(7, 8, 9);

    }

}
```

Após isso, adicionamos mais um método afim de fixar o conteúdo.


```java
public class Quadrilatero {

    public static void area(double lado) {

  

        System.out.println("Área do quadrado: " + lado * lado);

    }

  

    public static void area(double lado1, double lado2) { // Tipo double 

  

        System.out.println("Área do retângulo: " + lado1 * lado2);

    }

  

    public static void area(double baseMaior, double baseMenor, double altura){

  

        System.out.println("Área do trapézio: " + ((baseMaior + baseMenor)*altura) / 2);

    }

  

    public static void area(float diagonal1, float diagonal2) { // Tipo float

  

        System.out.println("Área do losango: " + (diagonal1 * diagonal2) / 2);

    }

  

}

```


Agora na classe Main: 
```java
public class Main {

  

    public static void main(String[] args) {

        // Quadrilátero

        System.out.println("Exeercício quadrilátero");

  

        Quadrilatero.area(3);

        Quadrilatero.area(5d, 5d); // Tipo double 

        Quadrilatero.area(7, 8, 9);

        Quadrilatero.area(7f, 8f); // Tipo float

  

    }

}
```

O intuiro era entender o porque é necessário a alteração dos tipos para que não ocorra erros de sitaxe.

É até possível que haja mais métodos, porém, com tipos diferentes, quantidades diferentes de tipos e até a ordem.
