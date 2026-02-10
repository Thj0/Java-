
## Objetivos 

1. Características da interface List;
	2. Como e quando utilizar ArrayList e LinkedList;
		3. Conhecer os principais métodos. 

___
# java.util.List


A interface List fica dentro do pacote java.util

Principais características da InterfaceList

 - Elementos duplicados e garante ordem de inserção

![[Pasted image 20260210184054.png]]

1° **Implementação Vector** - Quando pensado em Threads se pensa na implementação Vector, por que ela é uma implementação Thread-Safety. Isso não quer dizer que, não conseguimos sincronizar as outras implementações.

2° **ArrayList** - Implementa de InterfaceList

3° LinkedList - Implementa tanto de InterfaceList quanto de InterfaceQueue, isso quer dizer que ela tem métodos tanto de InterfaceList quanto InterfaceQueue. 

___
# Quando escolher e, Qual é a melhor? 

Na dúvida, sempre optar pelo ArrayList. 

![[Pasted image 20260210190636.png]]


"ArrayList deve ser usado onde mais operações de pesquisa são necesárias, e LinkedList deve ser usado onde mais operações de inserção e exclusão são necessárias."

___
# ArrayList 

Esta classe usa um array dinâmico para armazenar seus elementos.
Com a introdução de generics, essa classe oferece suporte ao armazenamento de todos os tipos de objetos.

Manipular um ArrayList leva mais tempo devido à sua implementação interna. 
Sempre que removemos um elemento, internamento o array é percorrido e os dados na memória são deslocados.

Esta classe implementa a interface List.
Portanto, ela atua como uma lista.

Esta classe funciona melhor quando a aplicação exige armazenar dados e acessá-los.

___
# LinkedList

Esta classe usa uma lista duplamente encadeada para armazenar seus elementos.
Assim como ArrayList, essa classe também suporta o armazenamento de todos os tipos de objetos.

Manipular uma LinkedList leva menos tempo em comparação ao ArrayList porque, em uma lista duplamente encadeada, não existe deslocamento de dados na memória.
A lista é percorrida e apenas as referências (links) são alteradas.

Esta classe implementa tanto a interface List quanto a interface Deque.
Portanto, ela pode atuar como uma lista e também como uma deque (fila de duas extremidades).

Esta classe funciona melhor quando a aplicação exige manipulação dos dados armazenados.

___
