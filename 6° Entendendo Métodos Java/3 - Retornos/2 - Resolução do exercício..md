
A ideia desse exercício é recriar a aplicação que calcula a área dos 3 quadriláteros notáveis, porém agora, com a intenção de que os métodos retornem valores.

Classe Quadrilátero: 
```java
/*Classe de exemplo para o exercício */

  

public class Quadrilatero {

  

    public static double area(double lado) {

  

        return lado * lado;

    }

  

    public static double area(double lado1, double lado2) {

  

        return lado1 * lado2;

  

    }

  

    public static double area(double baseMaior, double baseMenor, double altura) {

  

        return ((baseMaior + baseMenor) + altura) / 2;

  

    }

  

}
```


Classe Main: 
```java 
public class Main {

    public static void main(String[] args) {

  

        // Retornos

        System.out.println("Exercício retornos");

  

        double areaQuadrada = Quadrilatero.area(3);

        System.out.println("Area do quadrado: " + areaQuadrada);

  

        double areaRetangulo = Quadrilatero.area(5, 5);

        System.out.println("Área do retângulo: " + areaRetangulo);

  

        double areaTrapezio = Quadrilatero.area(7, 8, 9);

        System.out.println("Área do trapézio: " + areaTrapezio);

    }

  

}

```
