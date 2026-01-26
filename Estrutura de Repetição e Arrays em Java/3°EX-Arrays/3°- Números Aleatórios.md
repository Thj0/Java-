
O Objetivo desse código é que o programa leia 20 números aleatórios (entre 0 e 100), e armazene-os num vetor. Ao final mostre os números e seus sucessores.

```java
import java.util.Random;

  
  

public class numerosAleatorios {

    public static void main(String[] args) {

        Random luck = new Random();                   // Inicializa a classe Random para gerar números aleatórios.

  

        int[] roleta = new int[20];                     // Criamos um array de inteiros com 20 posições.

        for(int i = 0; i < roleta.length; i++){       // i recebe 0, indicando a primeira posição do array, e enquanto i for menor que o tamanho do array roleta, incremente 1 à i.

            int numero = luck.nextInt(100);    // Gera um número aleatório entre 0 e 99.

            roleta[i] = numero;                      // Roleta na posição i, recebe o número gerado por random

        }

  

        System.out.print("\nAntecessores dos números aleatórios: ");

        for (int numero : roleta) {

            System.out.print((numero-1) + " ");

        }

        System.out.print("\nNúmeros aleatórios: "); // Mensagem Ilustrativa

        for (int numero : roleta) {                 // Onde vamos navegar dentro do array

            System.out.print(numero + " ");         // Onde vai ser impresso os números aleatórios

        }

  

        System.out.print("\nSucessores dos números aleatórios: ");

        for (int numero : roleta) {

            System.out.print((numero+1) + " ");

        }

    }  

}
```