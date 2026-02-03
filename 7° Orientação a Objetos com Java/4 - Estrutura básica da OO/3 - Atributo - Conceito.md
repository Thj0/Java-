

"É o elemento de uma classe responsável por definir sua estrutura de dados. O conjunto destes será responsável por apresentar suas características e fará parte dos objetos criados a partir da classe"

É através dos atributos que a gente caracteriza as nossas classes e futuros objetos.

A primeira coisa que a gente pode colocar dentro de uma classe são seus atributos, que são características que vamos utilizar para representar/caracterizar o conceito do mundo real que queremos modelar.

Então tudo que diz respeito à características sobre conseguirmos representar o mais fielmente possível um conceito do mundo real, vamos ter que começar a definir atributos dentro da nossa classe.

**Ex:**

Bola
- Diâmetro 
___
Carro 
 - Cor
___
Venda
- Distância
___
Viagem 
 - Valor
___
Comprador 
- Nome
___
Computador 
 - Memória
___
Perceba que esses atributos estão caracterizando e tornando mais fino, o processo de representação desses conceitos. Estamos tentando representar da forma mais próxima do mundo real esses conceitos.


É para isso que serve os atributos, para caracterizarmos de uma forma mais fiel, os conceitos do mundo real.

____
### Atributo x Variável

Atributo:
	O que é próprio e peculiar a alguém ou a alguma coisa.

Variável:
	Sujeito a variações ou mudanças; que pode varias; inconstante, instável.


Na orientação a objetos utilizamos os dois, já na programação estruturada se trabalha mais com variáveis globais ou variáveis locais dentro das funções. 

Entretanto na Orientação a Objetos trabalhamos com ambas, tanto atributo quanto variável. 

Pode se dizer que, dentro do software do computador, tanto variável quanto atributo vão ser reconhecidos da mesma maneira, mas conceitualmente são diferentes.

Na OO, dentro das classes a gente cria atributos.
As variáveis nas linguagens OO, são definidas ou tem seu ciclo de vida dentro de métodos.

Atributos são criados dentro de classes. 

Conceitualmente, variáveis tem um ciclo de vida muito mais curto, é algo que utilizamos durante a execução de operações.

Agora, para representar um conceito do mundo real, utilizamos atributos.

___

- Dicas: 

Substantivos e adjetivos;
	A função dos adjetivos é caracterizar os substantivos para que consigamos definir da melhor forma possível, nossa classe/conceito do mundo real.
	
Nomes significativos;
	Entender o nicho do qual estamos tratando para poder definir melhor os atributos e seus valores.
	
Contexto deve ser considerado;
	Assim como a abstração, não devemos definir todos os atributos possíveis que um objeto pode ter, ou que uma classe pode ter; Pois podemos estar definindo coisas desnecessárias.
	Por isso devemos considerar o contexto da nossa classe, para poder definir exatamente os atributos que são essenciais.
	 
Abstração;
	
	
Tipos adequados.
	Entender qual a finalidade daquele atributo, para entender qual é o tipo de dado adequado para ele.

___

 - **Códigos:**

```Java
class Carro { 
	int portas;
}
```
___
```C#
class Carro { 
	int portas;
}
```
___
```Python
class Carro:
	portas = 0
```
___

# Exercício  - 2.

Evolua o exercício 1 e defina 3 atributos para sua classe "Carro": 

Cor;
Modelo;
Capacidade do tanque.


Obs: Utilize a linguagem que gosta e siga as dicas sobre como criar atributos.