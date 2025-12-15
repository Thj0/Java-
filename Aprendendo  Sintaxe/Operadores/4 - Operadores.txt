# Operadores

Incrementação está muito associada a recorrência de atribuição de um mesmo valor.

**O que é incrementar?**

É pegar um valor atual e aplicar uma nova atribuição desse valor. Considerando que esse incremento é sempre um valor igual 

Quando trabalhamos com incrementação, para operações curtas ou básicas, criamos uma variável e somamos ela com o incremento da mesma variável adicionando 1.



Exemplo:

int numero = 5;

numero = numero +1; 

System.out.println(numero);

Que resulta no número 6



Porém de uma forma mais prática e que serve para operações mais extensas, se utiliza a regra de incrementação.



int numero = 5;

System.out.println( ++ numero); ou System.out.println( numero ++)

Que resulta também no número 6

____

### A decrementação funciona da mesma forma



int numero 5;

numero = numero -1;

System.out.println(numero);

Que resulta no número 4

Agora utilizando a mesma forma, com a regra dos sinais exigida;



int numero = 5;

System.out.println( -- numero); ou System.out.println( numero -- )

Que também resulta no numero 4.

____

### É importante lembrar que;

**Incremento não é só atribuição, é um operador.**

Sobre eu dizer que o incremento/decremento é uma "recorrência de atribuição", não está errado, mas tecnicamente:



- numero = numero +1; - Atribuição 



- ++numero ou numero++ - Operador de incremento 



Eles fazem a mesma coisa no valor final, mas não se comportam igual em todas as situações .

____

**Existe diferença entre pré e pós incremento.**

Isso é importante quando o valor é usado na mesma linha.



int numero = 5;

System.out.println( ++ numero);

Incrementa antes de usar o valor.



int numero = 5;

System.out.println(numero ++ )

Usa o valor primeiro e incrementa depois.



No fim da execução, o valor do número será 6 nos dois casos, mas o que é impresso muda.

____



## Valores booleanos



Quando declaramos, ou temos uma variável de valor booleano, normalmente só é possível obter dois valores: true ou false

Para trabalhar com valores booleanos, também podemos utilizar **operadores unários**, como o operador de **negação lógica (`!`)**, que inverte o valor da variável.

### 

Exemplo: 

boolean variavel = true;

System.out.println(variavel);



O resultado será true.



Porém ao utilizarmos o operador denegação lógica ( ! ), o resultado muda, pois o valor é invertido.



boolean variavel = true; - Essa variável é em memória 

System.out.println(!variavel) 

Que resulta em false.



⚠️ **Importante**: nesse caso, **a variável original em memória não é alterada**. Apenas o valor exibido foi negado. A variável `variavel` continuará sendo **true** até que um novo valor seja atribuído a ela.

____

### Para que ela seja de fato false;

Teremos que reatribuir o valor à própria variável, porém negando-a (Utilizando a negação).



Exemplo:



boolean variavel = true;

variavel = !variavel;

System.out.println(variavel);



A variável deixou de ser true e passou a ser false, e o resultado impresso será **false**.

____



📌 **Resumo mental**:

- `!variavel -` apenas nega o valor **naquele momento.**
- `variavel =  !variavel` - altera o valor **armazenado em memória**.