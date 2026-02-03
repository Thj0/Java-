
"É uma porção de código (sub-rotina) que é disponibilizada pela classe. Este é executado quando é feita uma requisição a ele. Um método serve para identificar quais serviços, ações, que a classe oferece. Eles são responsáveis por definir e realizar um determinado comportamento."


Um método é usado para prover quais ações podemos utilizar.
Além de manipular os atributos da classe, trabalhando até mesmo com variáveis.
___
**Ex:**

Carro
 - ligar
___
Venda
 - calcularTotal
___
Comprador
 - realizarTroca 
___
Computador
 - desligar
___

Estes são alguns exemplos. Porém, não é porque o conceito de Orientação à Objetos existe que, temos de utilizá-lo por obrigação, - Não, podemos usar a depender da situação, se for necessário, sem problemas, se não for, sem problemas também. Ou seja, de acordo com o contexto. 

___

### Criação 

| Java e C#      |     | Python       |
| -------------- | --- | ------------ |
| - Visibilidade |     | - def        |
| - Retorno      |     | - Nome       |
| - Nome         |     | - Parâmetros |
| - Parâmetros   |     |              |

___
- **Dicas:**

Verbos;
	Os métodos são ações, comportamentos/operações.

Nomes significativos;
	Ajuda a definir melhor dentro do contexto.
	
Contexto deve ser considerado.
	

___
- **Códigos:**

```Java
class Carro{ 
	void frear() {
	
	...
	}
}
```
___
```C#
class Carro { 
	void frear(){
	
	...
	}
}
```
___
```Python
class Carro:
	def frear()
	
	
	
```
___

 - **Dois métodos especiais:**

- Construtor
	O que é um método construtor em Java?
	
	O construtor é um método especial que serve para inicializar um objeto.
	Ele é executado automaticamente quando se usa o `new` para criar um objeto.

	Como identificar um construtor?
	
	 Um construtor tem 3 características importantes:
	 
	 1. Tem o mesmo nome da classe;
	 2. Não tem retorno (nem void);
	 3. Geralmente serve para atribuir valores iniciais aos atributos.

 - Destrutor
	 
	 Em programação orientada a objetos, um destrutor é um método usado para "destruir" um objeto, ou seja, liberar recursos quando ele não será mais usado (memória, arquivos, conexões etc.).
	 
	Mas em Java NÃO existe destrutor como em outras linguagens (ex: C++).
	  
	Então como Java "destrói" objetos? 
	Java usa algo chamado **Garbage Colletor (GC)**. 
	
	O **Garbage Colletor** é um mecanismo automático que:
	
	 - Identifica objetos que não estão mais sendo usados;
	 - Libera a memória deles sozinho;
	 - O programador não precisa chamar nada
	 
	Em Java, você não destrói objetos manualmente.
	
___
### Construtor

A finalidade de um construtor é criar objetos.
Entretanto pode também, caso necessário, alguns valores iniciais para os atributos das nossas classes e também para os objetos que criamos.

Caso eu queira, posso criar um construtor e passar alguns parâmetros a ele para que ele guarde esses atributos

Mesmo que não iniciemos o construtor, ou seja, não criemos nenhum, a linguagem nos prove por debaixo dos panos um construtor padrão automaticamente (sem parâmetros).

Mas: 

Se criarmos qualquer construtor, o Java não cria mais o padrão de forma automática.

```Java
class Carro   {
	Carro () {
	
	...
	}
}
```


___
```C#
class Carro   {
	Carro () {
	
	...
	}
}
```


___
```Python
class Carro:
	def __init__(self):
	...
```


___

### Destrutor 




```Java
class Carro { 
	void finalize () {
	
	...
	}
}
```


___
```C#
class Carro { 
 ~Carro() {
 
 ...
 }
}
```


___
```Python
class Carro: 
	def __del__(self):
	...
	
```


___