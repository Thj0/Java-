

## Objetivo 

Fazer um programa que peça N números inteiros. Além de calcular e mostrar a quantidade de números pares e a quantidade de números ímpares.

## Método Utilizado: 

 - Do-While.

___

```Java 
import java.util.Scanner;

  

public class imparOuPar {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

  

        System.out.println("Quantos números você deseja digitar? ");
        int n = sc.nextInt();

  

        int impares = 0;
        int pares = 0;
        int contador = 1;

  

        do {
            System.out.println("Digite o " + contador + "° número.");
            int numero = sc.nextInt();

  
            if (numero % 2 == 0) {
                pares++;

            } else {
                impares++;

            }

  

            contador++;
        } while (contador <= n);

        System.out.println("Quantidade de números ímpares: " + impares):
        System.out.println("Quantidade de números pares: " + pares);

  

        sc.close();
    }
}
```

___ 
Explicação 

- Estrutura do-while
```Java
do { 
	//O código vai executar pelo menos 1 vez.
	
} while (condição);
```

A diferença do 'while', é que a condição só é testada no final.

___
 -  O controle do laço 
```Java 
int contador = 1;
```

```Java 
contador++;
```

```Java
while (contador <= n); 
```

Essas informações garantem que: 

1. O laço execute exatamente N vezes.
2. Cada número digitado seja contado corretamente.

___
 - Contagem de pares e ímpares 

```Java 
if (numero % 2 == 0){ 
	pares++;
} else { 
	impares++;
}
```

Aqui estou sendo simples e direto: 

1. Se o resto(%) for 0 - par
2. Senão, resto(%) diferente de 0 - ímpar

___
Após isso: 

```Java 
contador++; // Incremento
```

Se o incremento do contador não for aplicado, o loop nunca termina.

O programa fica repetindo o mesmo bloco para sempre.

**Ex.** Sem o incremento no contador
```Java
int contador = 1;


do {
    System.out.println("Executando");
    // contador++  ❌ ESQUECIDO
} while (contador <= n);
```

```
contador <= n  // sempre verdadeiro
```

Então ao rodar:

**Execução:**

1. O `do` **executa o código**
2. Chega no `while (contador <= 5)`
3. Pergunta: `1 <= 5` → **true**
4. Volta pro `do`
5. Executa de novo
6. Nada muda…

O resultado é um loop infinito.

Deixando o programa preso nesse ciclo.

___
## Como acontece um loop infinito?

Acontece quando um laço nunca termina, ou seja: 

O loop não termina porque a condição de parada nunca fica falsa.
Com isso o programa fica repetindo o mesmo bloco para sempre.

___
While 
```Java 
} while (contador <= n);
```

Na linha do while, dentro dos parênteses, está a condição de repetição do 'do-while'. 

Traduzindo: 

"Repita tudo que está dentro do 'do' "enquanto" contador for menor ou igual a "n". 

___
O java interpreta isso dessa forma: 

1. o bloco do {...} executa 
2. chega na linha do while 
```java 
contador <= n 
```
3. Se for true - volta pro do
4. Se for false - sai do loop


____
E o que acontece depois que o loop termina? 

Quando a condição vira false, o Java pula para a próxima linha fora do laço: 

```java
System.out.println("\nQuantidade de números pares: " + pares);
System.out.println("Quantidade de números ímpares: " + impares);
```


## Essas linhas fazem o quê?

Primeira impressão:

`System.out.println("\nQuantidade de números pares: " + pares);`

- \n - pula uma linha (quebra de linha)
- Concatena texto + valor da variável 'pares'
- Mostra o **total acumulado** durante o laço

Segunda impressão

`System.out.println("Quantidade de números ímpares: " + impares);`

Mostra quantos números **não eram pares**.
___

**Importante**:  
Essas linhas não fazem parte do laço, então:

- executam **uma única vez**
- só depois que todos os números foram digitados

___
Fechamento do Scanner
```java
sc.close();
```

### Pra que serve?

- Libera o recurso de leitura do teclado
- Boa prática em Java
- Evita avisos e possíveis problemas futuros

Depois de fechado, **não pode mais usar** `scanner.nextInt()`.
___

## Visão geral (fluxo do programa)

1. Entra no `do`
2. Lê número
3. Atualiza pares ou ímpares
4. Incrementa contador
5. Testa `contador <= n`
6. Se **true** - volta ao `do`
7. Se **false** - sai
8. Imprime resultados
9. Fecha o Scanner
10. Programa termina

____
