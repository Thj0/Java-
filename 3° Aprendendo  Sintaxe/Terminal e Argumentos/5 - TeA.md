
# Scanner 

Nos exemplos anteriores percebemos que podemos receber dados digitados pelo usuário do nosso sistema, porém precisa estar em uma linha e também é necessário informar os valores nas posições correspondentes. Esta abordagem pode deixar margens de execução com erro do nosso programa. Para isso, com a finalidade de deixar as nossas entradas de dados mais seguras vamos receber dados via **Scanner**. 

A classe **Scanner** permite que o usuário tenha uma interação mais assertiva com o nosso programa, veremos como vamos mudar o nosso programa **AboutMe** para deixar mais intuitivo aos usuários.

```Java 
import java.util.Locale; 
import java.util.Scanner;

public class AboutMe {
	public static void main(String[] args) {
		//criando o objeto scanner
		Scanner scanner = new Scanner(System.in).useLocale(Locale.US)
		
		System.out.println("Digite seu nome");
		String nome = scanner.next();
		
		System.out.println("Digite seu sobrenome");
		String sobrenome = scanner.next();
		
		System.out.println("Digite sua idade");
		int idade= scanner.nextInt()
		
		System.out.println("Digite sua altura");
		double altura = scanner.nextDouble();
		
	}
}
```


Uma das finalidades do Scanner, é obter parâmetros de entrada da nossa aplicação via terminal para que a gente possa ter uma melhor experiência ao executar nosso programa. 