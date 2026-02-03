
## Objetivo

Fazer um programa que leia conjuntos de dois valores, o primeiro representa o nome do aluno e o segundo representando a idade. (O programa tem que ser interrompido caso o valor 0 seja inserido no campo "nome").

## Método Utilizado: 

 - While.

____
```java
import java.util.Scanner;

  

	public class nomeIdade {

  

    //Esse exercício foi feito com a intenção de utilizar o "while" com uma condição de parada com break.

  

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);  

        System.out.println("Informe seus dados.");

  
  

        String nome;

        int idade;                              

  

        while (true){ //Enquanto for true/verdadeiro, execute:

  

        System.out.println("Nome: ");// Mensagem no terminal que pede uma informação.

        nome = sc.next();//O comando 'sc.next' faz com que o sistema de leitura, leia uma string.

        if (nome.equals("0")) break;// O break interrompe o loop caso o usuário digite '0' como nome.

  

        System.out.println("Idade: ");//Outra mensagem no terminal que pede uma segunda informação.

        idade = sc.nextInt();//Já o sc.nextInt' faz com que leia um valor inteiro.

        }

        System.out.println("Informe corretamente!");  // Mensagem exibida após o encerramento do loop.

        sc.close(); 
        // E aqui, após todo o código a gente fecha o sistema de leitura.

  

    }

}
```
