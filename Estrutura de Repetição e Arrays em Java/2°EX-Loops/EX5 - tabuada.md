
## Objetivo

Desenvolver um gerador de tabuada, capaz de gerar uma tabuada de qualquer número inteiro entre 1 à 10. O usuário deve informar qual número ele deseja ver a tabuada. A saída deve ser conforme o exemplo abaixo: 

Ex. Tabuada do 5: 

5 x 1 = 5
5 x 2 = 10 
5 x 3 = 15
... 
5 x 10 = 50


## Método Utilizado: 

 - For.

___
```java
import java.util.Scanner; // Import do sistema de leitura

  
  

public class tabuada {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in); // Início do sistema de leitura

  

        System.out.println("Tabuada do: " ); // Mensagem exibida ao usuário, para saber sobre qual tabuada ele deseja

        int multiplicador = sc.nextInt();       // Variável do tipo inteiro, que determina o número da tabuada

  

        for(int numero = 1; numero <= 10; numero++){  

        /*  Iniciando for/para. O for funciona em 3 etapas, inicialização, condição e incremento.

        *  1°- int numero recebe(=) 1;

        *  2°- enquanto 'numero' for menor ou igual(<=) à 10;

        *  3°- é acrescentado +1 ao valor de 'numero' - (++ significa +1)

        */

            int total = numero * multiplicador; // Criei a variável total, para que ela seja responsável pelo valor da multiplicação dos números

            System.out.println(multiplicador + " " + "x" + " " + numero + " = " + total); //Saída elaborada para que nos informe sobre todas as operações da tabuada.

  

        /*     if (multiplicador > 10) break; //Condição imposta para que o loop tenha um fim. Caso multiplicador ultrapasse o valor de 10 o loop é encerrado.

        Atualizando sobre o if...

        Eu entendi que o if não tem sentido, ou melhor, é desnecessário.

        Ele só seria útil caso eu quisesse impor uma condição específica, onde eu não gostaria que o usuário executasse.

        Ex: Um número, texto, ou qualquer outra coisa.

        Ou caso fosse uma condição que dependesse de algo que mudaria dentro do loop, ou, o loop.

        */

        }

  

        sc.close(); //Onde encerramos o sistema de leitura.

    }

}
```