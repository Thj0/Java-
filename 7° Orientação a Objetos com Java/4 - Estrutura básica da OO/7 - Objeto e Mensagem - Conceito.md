
"Um objeto é a representação de um conceito/entidade do mundo real, que pode ser física (bola, carro, árvore e etc.) ou conceitual (viagem, estoque, compra, etc...) e possui um significado bem definido para um determinado software. Para esse conceito/entidade, deve ser definida inicialmente uma classe a partir da qual posteriormente serão instanciados objetos distintos." 

Embora o objeto seja o principal foco do paradigma da programação orientada a objetos, tudo começa com a classe.
Entretanto são diferentes, a "classe" é uma coisa estática é como um molde, a gente define uma classe com a intenção de como criar/desenvolver, e manipular os objetos. Então o que executa de fato são os objetos, a classe permanece estática/parada.

Para que ela funcione, devemos criar objetos a partir dela. São esses objetos que estarão na memória do computador e farão as coisas acontecerem. 

São os objetos que vão armazenar os métodos, e os valores. 

A classe é algo estático que serve só de molde para criarmos objetos distintos. Objetos são instâncias de classes.

___ 
 - **Criação:**

```Java
Carro carro = new Carro ();
```

___
```Python
carro = Carro ()
```

___
```C#
Carro carro = new Carro ();
```

___
# Mensagem 

"É o processo de ativação de um método de um objeto. Isto ocorre quando uma requisição (chamada) a esse método é realizada, assim disparando a execução de seu comportamento descrito por sua classe. Pode também ser direcionada diretamente à classe, caso a requisição seja a um método estático."

É a troca de mensagens entre objetos e classes que fazem o sistema funcionar.

**Ex:**

```Java 
Carro carro = new Carro(); // Onde criamos um objeto 
carro.<método>;            // Onde usamos um objeto para chamar um método
// Porém, se a mensagem é para a classe 
Carro.<método>;            // Usamos a classe para chamar um método
```

```Python
carro = Carro()
carro.<método>

Carro.<método>
```

```C#
Carro carro = new Carro();
carro.<método>;

Carro.<método>;
```


___
**Conceitos Mais avançados**

 - Instância x Estático: atributos e métodos
	 Importante entender o que são atributos de instância e atributos estáticos, e métodos de instância e métodos estáticos. 
	 Essas são as duas formas que os atributos e métodos podem se comportar, e entender como cada um desses funcionam ajuda muito a saber quando utilizar cada um.
	 
 - Estado de um Objeto
	Também é importante entender o que define um estado de um objeto e pra que serve.
	Basicamente pode se dizer que o estado de um objeto diz respeito aos valores dos seus atributos.
	
 - Identidade de um Objeto 
	Também é importante entender o que é, 'identidade de um objeto' o por quê nós precisamos identificar de forma única um objeto e como podemos fazer isso.
	
 - Representação numérica de um objeto
	Geralmente essa representação trabalha em conjunto com a identidade de um objeto. Toda vez ao percebermos que é necessário trabalhar com a identidade de um objeto, vai ser importante definir a representação numérica desse objeto. 
	
	"Identidade de um Objeto" e "Representação numérica de um Objeto", esses dois assuntos sempre caminham juntos. 
	
 - Representação padrão de um objeto
	As vezes um objetos no qual estamos trabalhando possuí muitos atributos e características, mas, algumas dessas podem ser utilizadas para representar de uma forma mais simples e que consiga identificar esse objeto de uma forma mais compreensível.
	
	Então a representação padrão de um objeto ajuda muito nisso. Uma forma de representar de uma forma mais compreensível aquele objeto.

___
# Exercício - 4

Evolua o conceito do exercício 3 criando objetos da classe "Carro".

Use os métodos set/get, quando aplicáveis, para definir os valores dos atributos e exibir estes valores "get". Passe também uma mensagem para o cálculo do total pra encher o tanque.

Obs: Use a linguagem que gostar e siga as dicas sobre como criar métodos, atributos, etc. 

Obs: Use System.out, Console.WriteLine ou print.