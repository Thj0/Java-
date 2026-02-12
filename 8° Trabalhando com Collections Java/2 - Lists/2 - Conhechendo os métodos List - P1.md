
Formas de se inicializar um List

```Java
class ExemploList {


//List notas = new ArrayList(); // Antes do Java5

//List<Double> notas = new ArrayList<>(); //Generics(jdk 5) - Diamont Operator(jdk 7)

//ArrayList<Double> notas = new ArrayList<>();

//List<Double> notas = new ArrayList<>(Arrays.asList(7d, 8.5, 9.3, 5d, 7d, 0d, 3.6));

//List<Double> notas = Arrays.asList(7d, 8.5, 9.3, 5d, 7d, 0d, 3.6));

}
```

```Java
package List;

  

import java.util.ArrayList;

import java.util.List;

  

public class ExemploList {

    public static void main(String[] args) {

        //Dada uma lista com 7 notas de um aluno [7, 8.5, 9.3, 5, 7, 0, 3.6 ], Faça:

        //List notas = new ArrayList(); // Antes do Java5

        //List<Double> notas = new ArrayList<>(); //Generics(jdk 5) - Diamont Operator(jdk 7)

        //ArrayList<Double> notas = new ArrayList<>();

        //List<Double> notas = new ArrayList<>(Arrays.asList(7d, 8.5, 9.3, 5d, 7d, 0d, 3.6));

        //List<Double> notas = Arrays.asList(7d, 8.5, 9.3, 5d, 7d, 0d, 3.6));

        //notas.add(10d);

        //System.out.println(notas);

  

  

    /*  List<Double> notas = List.of(7d, 8.5, 9.3, 5d, 7d, 0d, 3.6);

        notas.add(1d);

        notas.remove(5d);

        System.out.println(notas);

    */

  

        System.out.println("Crie uma lista e adicione as sete notas: ");

        List<Double> notas = new ArrayList<>(); //Generics(jdk 5) - Diamont Operator(jdk 7)

        notas.add(7.2);

        notas.add(9.3);

        notas.add(8.7);

        notas.add(6.9);

        notas.add(5.0);

        notas.add(4.5);

        notas.add(1.3);

  

        System.out.println(notas.toString());

  

        System.out.println("Exibo a posição da nota 5.0: " + notas.indexOf(5d));

  

        System.out.println("Adicione na lista a nota 8.0 na posição 4: ");

        notas.add(4, 8d); //O Método 'add' para adicionar, introduz primeiro o índice, depois o elemento.

        System.out.println(notas);

  

        System.out.println("Substitua a nota 5.0 pela nota 6.0: ");

        notas.set(notas.indexOf(5d), 6.0); //O Método 'set' para subtituir, primeiro recebe a posição para substituição, e depois o elemento.

        // O método 'indexOf' nos informa a posição de determinado número ou informação, e depois passamos a característica do substituto.

        System.out.println(notas);

  

        System.out.println("Confira se a nota 5.0 está na lista: " + notas.contains(5d));

        //notas.contains(); - O método 'contains' é utilizado para checagem, eu informo o objeto que procuro e ele me retorna um valor boolean.

  

        System.out.println("Exiba todas as notas na ordem em que foram iseridos: ");

        for (Double nota: notas)

        System.out.println(nota);

  
  

    }

}
```