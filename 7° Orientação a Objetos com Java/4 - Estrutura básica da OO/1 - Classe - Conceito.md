# Objetivos 

1 - Apresentar os conceitos que criam as estruturas básicas da OO:

Classe
Atributo
Método
Objeto
Mensagem

Tudo na Orientação a Objetos começa por esses conceitos.
Por isso são chamadas de estruturas básicas, pois são essenciais.

___
# Classe

"É uma estrutura que abstrai um conjunto de objetos com características similares. Uma classe define o comportamento de seus objetos através de métodos e os estados possíveis destes objetos através de atributos. Em outros termos, uma classe descreve os serviços providos por seus objetos e quais informações eles podem armazenar."

A finalidade da classe, é servir de molde.
É através da classe que vamos modelar o nosso determinado conceito do mundo real.

Quando falamos de modelar, entende-se que vamos modelar essa classe de uma forma que ela vai criar vários objetos dessa entidade do mundo real, abstraindo características similares.

Abstração é se preocupar com as características essenciais.

E é a partir desse pensamento que conseguimos criar classes, para a partir dessas classes criarmos objetos. 
___
- **Ex:** 

Bola; - Concreto
Carro; - Abstrato
Venda;
Viagem;
Comprador;
Computador.

Com uma classe podemos representar ambos, seja concreto ou abstrato. 
___
- **Dicas:**

- Substantivos;
- Nome significativos;
- Contexto deve ser considerado.

De acordo com a necessidade de cada software, vamos identificar essas entidades/substantivos para poder definir classes, pra poder representar eles dentro do nosso sistema.
___
 - **Códigos:**

```Java
class Carro { 
}
```
___
```C#
class Carro { 
}
```
___
```Python
class Carro:
	pass
```
___
Nem toda linguagem segue todos os conceitos da Orientação à Objetos.

Cada linguagem tem a liberdade de implementar a Orientação à Objetos de um determinado jeito e maneira, de acordo com as características da própria linguagem.

E assim como mostrado acima, essa é a forma mínima de definir classes vazias nessas linguagens.
___
