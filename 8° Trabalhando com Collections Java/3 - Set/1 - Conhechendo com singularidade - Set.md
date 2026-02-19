

1. As características da interface Set 

2. Como e quando utilizar HashSet, LinkedHashSet e TreeSet 

3.  Conhecer os principais métodos

___
# java.util.Set


Assim como a interface List, a interface Set a gente encontra no pacote, "java.util". 

Porém diferente da interface list, a interface set: 

- Não permite elementos duplicados
- Não possui índice 

Na interface Set a gente não consegue fazer o método 'set', onde a gente passa a posição e passa o elemento que a gente quer que seja substituído.

A gente não consegue fazer pesquisas em um método que precise de índices.




![[Pasted image 20260219150305.png]]



TreeSet implementa de 

<< InterfaceNavigableSet >> que implementa de 

<< InterfaceSortedSet >> que é extends de 

<< InterfaceSet >>

É um caminho de muitos métodos.

Precisaremos bastante do TreeSet quando precisamos fazer ordenação.

___
A implementação HashSet é que implementa diretamente de 

<< InterfaceSet >> 

Já a LinkedHashSet ela extend de HashSet


___
![[Pasted image 20260219151510.png]]
### HashSET 

HashSet usa internamente HashMap para armazenar seus elementos.
HashSet não mantém nenhuma ordem dos elementos.
HashSet oferece melhor performance que LinkedHashSet e TreeSet.
HashSet permite no máximo um elemento null.

___
### LinkedHashSet

LinkedHashSet usa internamente LinkedHashMap para armazenar seus elementos.
LinkedHashSet mantém a ordem de inserção dos elementos.
A performance do LinkedHashSet fica entre HashSet e TreeSet.
LinkedHashSet também permite no máximo um elemento null.

___
### TreeSet

TreeSet usa internamente TreeMap para armazenar seus elementos.
TreeSet mantém a ordenação natural padrão (ordem crescente).
TreeSet tem performance menor que HashSet e LinkedHashSet.
TreeSet não permite nem um único elemento null.

___
