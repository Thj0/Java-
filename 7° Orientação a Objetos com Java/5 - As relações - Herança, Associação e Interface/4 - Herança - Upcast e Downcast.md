
 - **Upcast e Downcast:**

![[Pasted image 20260204184123.png]]

Funcionário - Classe mãe.

Gerente - Subclasse.
Vendedor - Subclasse.
Faxineiro - Subclasse.

Todos esses são funcionários.
Cada um tem suas atividades, porém são especializações, subtipos de funcionário.

Upcast:
	Subir os tipos
	Subir na sua hierarquia de classe.
	
	Ex: 
	Se eu subo gerente e transformo em um funcionário, eu estou fazendo um upcast.
	
	E isso é possível porque gerente é um funcionário.

Downcast:
	É justamente o oposto.
	Eu desço o meu tipo.
	
	Desço na hierarquia de classe.
	Nesse caso eu transformo funcionário em:
	Gerente, Vendedor e Faxineiro.
	
	É o caminho pra baixo na hierarquia.

Até chegar na classe genérica.
___
 - Upcast.

O upcast é sempre implícito, ou seja, eu não preciso realizar uma transformação explícita e que visualmente amostra.


```Java 
//A superclasse, B subclasse de A 

A a = new B();  // B extends A
	            // Estou transformando B em A - Upcast
```

___
```C#

A a = new B();

```

___
```Python

```
Python não trabalha com essa ideia de Upcast.

___
- Downcast: 

No Upcast a gente transforma a classe filha na classe mãe, porém, no downcast a gente transforma a classe mãe na classe filha.


Já o downcast é explícito, eu tenho que dizer pra quem eu quero transformar.

```Java

B a = (B) new A(); // new A, transformo pra (B) e armazeno na variável do tipo B

```

___
```C#

B b = (B) new A();

```

___
```Python



```
Em python não se utiliza o downcast.

___

Entretanto utilizar o downcast no dia a dia não é muito recomendável, pois pode acontecer de conter muitos erros tanto de compilação quanto de execução.


Somente é útil quando trabalhamos com a classe object, pois não é tão provável de haver erros.
___
