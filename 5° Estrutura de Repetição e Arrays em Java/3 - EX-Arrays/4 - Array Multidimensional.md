
O Objetivo desse exercício foi fazer um programa que gere uma matriz 4x4 com valores aleatórios entre 0 e 9.

Nesse exercício utilizamos também os métodos:

 - for;
 - foreach. 

Além de trabalhar com a classe "Random", que gera números aleatórios.

```java
import java.util.Random;

  

/*O objetivo desse exercício é fazer um programa em que gere e imprima uma matriz M 4x4 com valores aleatórios entre 0-9*/

  

public class arrayMultidimensional {

    public static void main(String[] args) {

        Random joker = new Random();         // Inicializando a classe random que vai nos gerar números aleatórios.

        int[][] M = new int[4][4];           // Criação de uma matriz de inteiros com 4 linhas e 4 colunas

  
  

        for(int i = 0; i < M.length; i++) {   // i representa as linhas do array, enquanto o índice de i for menor que o tamanho do vetor, incrementa 1 à i.

            for(int j = 0; j < M[i].length; j++) { // j representa as colunas, enquanto a posição de j for menor que o elemento do vetor, incrementa 1 à j.

                M[i][j] = joker.nextInt(10);  // Integro as linhas e os elementos ao vetor, e peço para classe gerar os números aleatórios entre 0 e 9.

            }

        }

  

        System.out.println("Matriz: "); // Mensagem ilustrativa

        for (int[] linha : M) {           // linha navega sobre o array linhas

            for (int coluna : linha ) {   // coluna que navega entre os elementos das linhas

                System.out.print(coluna + " "); // imprime os números em linhas e colunas

            }

            System.out.println();

        }

    }

}
```



