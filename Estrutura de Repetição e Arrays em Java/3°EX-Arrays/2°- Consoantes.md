
O objetivo desse exercício é fazer um programa que leia um valor de 6 caracteres, e diga quantas consoantes foram lidas. E obviamente que, imprima as consoantes.

Nesse exercício foi utilizado um método de string,o método se chama `equals.IgnoreCase`

Esse método compara strings, se for igual retorna true, e se for diferente retorna false.
Além disso esse método não se importa se a letra ou string for maiúscula ou minúscula.

Ex: 
Se e letra que coloquei dentro do método for a, independente se o usuário digitar a letra 'a' de forma maiúscula ou minúscula, vai ser true, porque é igual.

___
Ainda nesse exercício utilizamos também o laço 'foreach'.

foreach é uma forma mais simples de percorrer (passar por) todos os elementos de um array ou coleção, um por um, sem usar índice.

Ele serve para ler os valores, não para controlar posições.

Ele percorre automaticamente todos os elementos de um array ou coleção, sem usar índice, tornando o código mais simples quando só precisamos acessar os valores.

```java 
import java.util.Scanner;

  

public class consoantes {

    public static void main(String[] args) {

        Scanner look = new Scanner(System.in);                 // Inicializando a entrada de fluxo de dados através do teclado

  

        String[] consoantes = new String[6];                   // Iniciando um array vazio com 6 posições

        int quantidadeConsoantes = 0;                          // Conta quantas consoantes foram digitadas.

        int contador = 0;                                      // contador serve como um controle do loop

        // Início do loop

        do {

            System.out.println("Letra: ");                  // Aqui é onde pede uma letra

            String letra = look.next();                       // Onde o sistema capta a letra digitada e atribui à variável letra.

  

            if(!(letra.equalsIgnoreCase("a") || // Se a letra NÃO for uma vogal (a,e,i,o,u), independente de maiúscula ou minúscula.

                 letra.equalsIgnoreCase("e") ||

                 letra.equalsIgnoreCase("i") ||

                 letra.equalsIgnoreCase("o") ||

                 letra.equalsIgnoreCase("u"))){

  

                consoantes[contador] = letra;                  // Atribua a letra ao elemento do vetor na posição indicada pelo contador, caso, seja consoante.

                quantidadeConsoantes++;                        // caso seja, acrescente 1 no valor de quantidadeConsoantes

  

            }

  

            contador++;                                        // Acrescente o valor 1 à variável contador, a cada loop.

  

        } while(contador < consoantes.length);                 // Enquanto contador for menor que o tamanho do array.

  

        System.out.println("Consoantes: ");                 // Mensagem ilustrativa

        for (String naoVogal : consoantes) {                  // Para cada naoVogal dentro do array consoantes.

            if(naoVogal != null)                              // Se o valor de naoVogal for diferente de null.

                System.out.println(naoVogal + " ");           // Imprima à naoVolgal

        }

        System.out.println("Quantidade de consoantes: " + quantidadeConsoantes);

        System.out.println(consoantes.length);                

  

        look.close();                                         // Encerrando a entrada de fluxo.

    }

}
```

