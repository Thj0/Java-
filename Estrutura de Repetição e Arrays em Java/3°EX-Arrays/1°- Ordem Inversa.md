
O Intuito do exercício é criar um vetor de números inteiros e que o programa mostre-os na ordem inversa.

Além disso aprendi sobre "lenght", length é uma propriedade do vetor que retorna o tamanho desse vetor.

Para descobrir o tamanho de um vetor, eu imprimo o nome dele com o ".length".
**Ex**: `System.out.println(select.length)` 

Serve para saber quantos elementos tem dentro desse vetor.
Se eu tenho um vetor com 7 elementos, a posição de número 7 não existe.

Navegando dentro do vetor, entendemos que ele não nos retornará o ultimo número como a representação literal do tamanho do vetor, Por quê? 

Porque um Array começa em 0, e sempre que quisermos consultá-lo teremos que esquecer do elemento 7, porém, não literalmente. Só que vamos sempre contá-lo como o 6 elemento, porque lembrando, eles começam em 0.

_____

```java 
public class ordemInversa {

    public static void main(String[] args) throws Exception {

        int[] select = {13, 18, 20, 24, 27, 28, 30};  //Determinamos um vetor do tipo inteiro com 7 elementos

        System.out.println("O vetor possui " + select.length + " elementos.");      // Nessa linha, informamos a quantidade de elementos que o vetor possui.

  

        int control = 0;                              // Control serve como um contador.

  

        System.out.println("Que são eles: ");

        while (control < select.length){              // Enquanto control for menor que o tamanho do vetor, o laço continua executando.

            System.out.print(select[control] + " ");  // Saída do código que mostra o vetor na posição de control

            control++;                                // Incrementa control em 1 a cada iteração do laço.

  

        }

  

        System.out.println("\nImpressão na ordem inversa.");   // Mensagem de saída do for  

        for (int tip = (select.length -1); tip >= 0; tip --){    // Para tip, ele recebe o último índice com length -1, enquanto tip for maior ou igual a 0, decremente

            System.out.print(select[tip] + " ");                 // Saída do resultado de for

  
  

        }

  

    }

}
```

