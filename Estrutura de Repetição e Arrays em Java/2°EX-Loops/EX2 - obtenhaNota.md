
## Objetivo 

Fazer um programa que peça uma nota, entre zero e dez. E que mostre uma mensagem caso o valor seja inválido e continue solicitando até que o usuário informe um valor válido.

## Método Utilizado: 

 - Do-While.

___
```java 
import java.util.Scanner;

  

//Esse exercício foi feito com a intenção de utilizar o "while".

/*A intenção é que o programa peça uma nota entre, zero e dez.

Além de mostrar uma mensagem caso o valor seja inválido, e que continue pedindo, até que o usuário informe um valor válido. */

  

public class obtenhaNota {

    public static void main(String[] args) {

  

        Scanner sc = new Scanner(System.in);

  

        System.out.println("Informe um número.");

  
  

        System.out.println("Sua nota é: ");

        int zeroDez = sc.nextInt();                           // Aqui ele lê um inteiro digitado pelo usuário

  

        while (zeroDez < 0 || zeroDez > 10) {                 // Enquanto @while zeroDez for menor(<) que 0, ou(||), zeroDez for maior(>) que 10, o loop é acionado.

            System.out.println("Informe corretamente!");   // O valor inválido, faz com que também exiba uma mensagem.

            System.out.println("Digite novamente: ");      // Exigindo que informe um valor dentro da condição imposta.

            zeroDez = sc.nextInt();                        

  

        }

        System.out.println("Obrigado pela colaboração!");

  

        sc.close();  // E encerramos aqui, o sistema de leitura.

  

    }

}
```
