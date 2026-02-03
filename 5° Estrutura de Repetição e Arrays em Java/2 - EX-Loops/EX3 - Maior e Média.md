
## Objetivo

Fazer um programa que leia 5 números e que informe o maior número, além de informar a média do valor total acumulado. 

## Método Utilizado: 

 - Do While.

____
```java
import java.util.Scanner;


public class maiorMedia{

	public static void main(String[] args){
		Scanner scan = new Scanner(System.in);
		
		int numero; 	
		int maior;
		
		int soma = 0;
		
		int contador = 0;
		do{ 
			System.out.println("Numero: ");
			numero = scan.nextInt();
			
			soma = soma + numero;
			
			if (numero > maior) maior = numero;
			
			contador = contador + 1;
		} while(contador < 5); 
			
			System.out.println("Maior: " + maior);
			System.out.println("Média: " + (soma/5));
		
		System.out println("Maior: " + maior);
	}
}



```