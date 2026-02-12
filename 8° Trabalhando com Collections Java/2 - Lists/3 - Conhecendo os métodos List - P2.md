
Continuação dos métodos List.
___

```Java
/*
O método Collection.min() retorna o menor elemento da Collection.
Ele funciona porque o tipo Double implementa Comparable,
permitindo comparação entre os elementos da lista 
*/
```

```Java
package List;

  

import java.util.ArrayList;

import java.util.Collections;

import java.util.Iterator;

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

  

        //System.out.println(notas.toString());

  

        //System.out.println("Exibo a posição da nota 5.0: " + notas.indexOf(5d));

  

        //System.out.println("Adicione na lista a nota 8.0 na posição 4: ");

        //notas.add(4, 8d); //O Método 'add' para adicionar introduz primeiro, o índice depois o elemento.

        //System.out.println(notas);

  

        //System.out.println("Substitua a nota 5.0 pela nota 6.0: ");

        //notas.set(notas.indexOf(5d), 6.0); //O Método 'set' para subtituir, primeiro recebe a posição para substituição e depois o elemento.

        // O método 'indexOf' nos informa a posição de determinado número e depois passamos a informação do substituto.

        //System.out.println(notas);

  

        //System.out.println("Confira se a nota 5.0 está na lista: " + notas.contains(5d));

        //notas.contains(); - O método 'contains' é utilizado para checagem, eu informo o objeto que procuro e ele me retorna um valor boolean

  

        //System.out.println("Exiba todas as notas na ordem em que foram iseridos: ");

        //for (Double nota: notas)

        //System.out.println(nota);

  

        System.out.println("Exiba a terceira nota adicionada: " + notas.get(2)); //'Get'  Método que recebe uma informação

        System.out.println(notas.toString());

  

        System.out.println("Exiba a menor nota: " + Collections.min(notas));

        /*Não existe um método nativo que exibe a menor nota, por isso utilizamos a classe 'Collections'

        junto ao método 'min' e passamos a nossa list 'notas' já que ela é uma collection.

        o 'min' é uma forma padrão que pega o menor valor em uma Collection.

        o min funciona com qualquer tipo que seja:

        comparable (ordem natural)

        ou

        tenha comparador informado.

        */

  

        System.out.println("Exiba a maior nota: " + Collections.max(notas));

        // funciona da mesma forma que o Collections.min(), porém pega o maior valor da Collection.

  
  
  

        Iterator<Double> iterator = notas.iterator();

        /*

        Utilizando o método iterator eu pego os valores desejados e realizo a soma de forma padrão.

        */

        Double soma = 0d;

        while (iterator.hasNext()) {

            Double next = iterator.next();

            soma += next;

        }

        System.out.println("Exiba a soma dos valores: " + soma);

  
  

        System.out.println("Exiba a média das notas: " + (soma / notas.size()));

        /*A média é a soma de tudo, dividido pela quantidade de elementos dentro a minha list.

        Com isso utilizamos o método size, para saber a quantidade exata de elementos.

        Size retorna um inteiro, com isso saberemos a quantidade de elementos. */

  

        System.out.println("Remova a nota 4: ");

        notas.remove(4.5);

        System.out.println(notas);

        /* remove é próprio para remoção de elementos

        posso passar tanto a sua posição quanto o próprio objeto.

        */

        System.out.println("Remova a nota da posição 0");

        notas.remove(0);

        System.out.println(notas);

  
  

        System.out.println("Remova as notas menores que 7 e exiba a lista: ");

        Iterator<Double> iterator1 = notas.iterator();

  

        while(iterator1.hasNext()) {

            Double next = iterator1.next();

  

            if(next < 7d) iterator1.remove();

        }

        System.out.println(notas);

  
  

        System.out.println("Apague toda a lista");

        notas.clear();

        //O método clear serve para limpar nossa collection, que no caso é a list.

        System.out.println(notas);

  

        System.out.println("Confira se a lista está vazia: " + notas.isEmpty());

        /*Esse método é um tipo boolean, ele me retorna true ou false se a lista estiver vazia ou não*/

  
  

    }

}


```

___
# Prática

Exercícios 

Resolva esses exercícios utilizando os métodos da implementação LinkedList: 

System.out.println("Crie uma lista chamada 'notas2' " + "e coloque todos os elementos da list ArrayList nessa nova lista: ")

System.out.println("Mostre a primeira nota da nova lista sem removê-lo: ");

Syste.out.println("Mostre a primeira nota da nova lista removendo-o: ");