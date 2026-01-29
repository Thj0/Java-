
# Objetivos 

1. Entender o que é sobrecarregar um método;

2. Saber como criar sobrecargas;

___
### Conceituação 

"É a capacidade de definir métodos para diferentes contextos, mas preservando seu nome."

Quando dizemos "definir métodos para diferentes contextos" 

Quer dizer que um mesmo método pode se comportar de forma diferente, de acordo com alguma necessidade, porém, preservando o seu nome.

Para que isso seja possível devemos mudar a lista de parâmetros do método, com isso conseguimos fazer esse mesmo método se comportar de forma diferente de acordo com cada contexto. 

Ex: 
Alterar a assinatura do método:
	Ass = nome + parâmetros

```java
converterParaInteiro(float f);
converterParaInteiro(double d);
converterParaInteiro(String s)
converterParaInteiro(float f, RoundType rd);
converterParaInteiro(double d, RoundType rd);
converterParaInteiro(String s, RoundType rd);
```
	converterParaInteiro (RoundType rd, String s);
	converterParaInteiro();


___
Ao mudar a lista de parâmetros, mantendo o nome do método preservado, saiba que foi criada uma sobrecarga.
___

Ex: 

https://docs.oracle.com/javase/7/docs/api/io/PrintStream.html


```java
void					println()
						Terminates the current line by writing the line separator.
						
void					println(boolean x)
						prints a boolean and then terminate the line.
						
void					println(char x )
						Prints a character and the terminate the line.
						
void					println(char[] x)
						Prints an array of characters and the terminate the line.
						
void					println(double x)
						Printsa double and then terminate the line.
						
void 					println(float x)
						Prints a float and the terminate the line.
						
void					println(int x)
						Prints an integer and then terminate the line.
						
void					println(long x)
						Prints a long and then terminate the line.
						
void					println(Object x) 
						Prints an Object and then terminate the line.
						
void					println(String x)
						Prints a String and then terminate the line.
```


O método 'println' é sobrecarregado. 

Outro exemplo: 

https://docs.oracle.com/javase/7/docs/api/java/lang/String.html

```java
static String		valueOf(boolean b)
					Returns the string representation of the boolean argument.
					
static String		valueOf(char c)
					Returns the string representation of the char argument.
					
static String		valueOf(char[] data)
					Returns the string representation of the cha array argument
					
static String		valueOf(char[] data, int offset, int count)
	Returns the string representation of specific subarray of the char argument. 
	
static String		valueOf(double d)
					Returns the string representation of the float argument.
					
static String		valueOf(float f)
					Returns the string representation of the float argument.
					
static String		valueOf(int i)
					Returns the string representation of the int argument.
					
static String		valueOf(long l)
					Returns the string representation of the long argument.
					
static String		valueOf(Object obj)
					Returns the string representation of the Object argument.
```

___

# Curiosidade

### Sobrecarga x Sobrescrita


Ambos são conceitos que atuam e são aplicados em cima de métodos, mas a forma de criar e de usar, e o modo como elas se comportam uma sobre a outra, são completamente diferentes.

___

# Exercitando 

Objetivo: Criar uma aplicação que calcula a área dos 3 quadriláteros notáveis, quadrado, retângulo e trapézio.

Obs: Usando sobrecarga.
