
# Objetivos da Aula 

1. O que são e porque usamos Collections Framework

2. Composição do Collections Framework

3. Hierarquia do Collections Framework.

___
# Collection


Collection é um objeto que agrupa múltiplos elementos (variáveis primitivas ou objetos) dentro de uma única unidade.

 Serve para armazenar e processar conjuntos de dados de forma eficiente.

 Antes do Java 2 (JDK 1.2), a implementação de coleções na linguagem Java incluía poucas classes e não tinha a organização de um framework.

___
# Composição Collections


**Interfaces:** É um contrato que quando assumido por uma classe deve ser implementado.

**Implementações ou Classes:** São as materializações, a codificação das interfaces.

**Algoritmos:** É a sequência lógica, finita e definida de instruções que devem ser seguidas para resolver um problema.

___

# Hierarquia Collections

![[Pasted image 20260210141924.png]]
  
As implementações e interfaces que vamos ver durante o curso: 

<< Interface - list >>
E suas implemetações;

ArrayList

LinkedList

___
<< Interface - Set >>
E suas implementações;

HashSet 

LinkedHashSet

___
<< Interface - Map >>
E suas implementações;

HashMap

LinkedHashMap

___
Falando sobre 2 implementações 

TreeSet e,
TreeMap.

Essas duas implementações elas tem como estrutura, por de baixo dos panos a estrutura de árvore binária.

Então, alguns métodos dentro dessas implementações tem herda o conceito de árvore.

___
Falando sobre **Vector** e **Hashtable**.

As implementações Vector e Hashtable são Thread safe.

Thread-safe em Java refere-se a classes ou métodos projetados para funcionar corretamente quando acessados simultaneamente por múltiplas threads. Eles garantem a integridade e consistência dos dados, evitando estados inválidos ou condições de corrida (race conditions) quando o estado compartilhado é lido ou alterado por várias partes do código ao mesmo tempo.

### Principais formas de alcaçar thread safety em Java

 - **Sincronização -** `(synchronized)`: Usa a palavra-chave `synchronized` em métodos ou blocos para permitir que apenas uma thread acesse o recurso por vez.

 - **Objetos Imutáveis:** Criar classes cujos estados não podem ser alterados após a criação, garante segurança, pois dados imutáveis não sofrem corrupção.

 - **Coleções Concorrentes** `(java.util.concurrent)`: Usar coleções especializadas como `ConcurrentHashMap` em vez de `HashMap`, que são otimizadas para acesso concorrente.

 - **Variáveis Locais e TrheadLocal:** Utilizar variáveis dentro do escopo do método, pois cada thread possui sua própria cópia, eliminando a necessidade de sincronização.

___
### Por que usar?

Sem o tratamento adequado de thread safety, aplicações multithread podem sofrer com a corrupção de dados e comportamento inconsciente, como em operações de incremento (`count++`) que não são atômicas. 

### Exemplos no Java

**Thread-safe:** `Vector`, `Hashtable`, `StringBuffer`, `ConcurrentHashMap`.

**Não Thread-safe:** `ArrayList`, `HashMap`, `StringBuilder`.

___
# Exercícios 


- Estude mais sobre a composição das collections: 
	1. Interfaces
	2. Implementações 
	3. Algoritmos.

 - Analise a Hierarquia do Collections Framework.
	
	


