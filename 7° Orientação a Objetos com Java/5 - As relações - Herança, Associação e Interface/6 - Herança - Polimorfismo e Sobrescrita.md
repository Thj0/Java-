
**Polimorfismo**

"A mesma ação, se comportando diferente."

-É a possibilidade de um mesmo método se comportar diferente.


O polimorfismo pode ser usado com herança, mas não é obrigatório. Porém, geralmente é bastante utilizado para se obter uma flexibilidade de ter uma mesma operação se comportando de uma forma diferente.

EX:
![[Pasted image 20260205124008.png]]

___
- Polimorfismo
	- Códigos: 
		- Ver exemplo

___
**Sobrescrita**

Um outro conceito relativo aos métodos, relacionado à herança. 

E o que é?

"A mesma ação, podendo se comportar diferente."


A diferença entre polimorfismo e sobrescrita é que o polimorfismo se comporta diferente, já a sobrescrita pode ou não se comportar diferente.

Polimorfismo - "se comportando diferente."

Sobrescrita - "podendo se comportar diferente."


![[Pasted image 20260205125112.png]]

___
 - Sobrescrita
	 - Códigos: 
		 - Ver exemplo

___
# Curiosidade

Polimorfismo x Sobrescrita

À primeira vista os dois são bastante parecidos, a manifestação desses conceitos em código são quase idênticas, mas, conceitualmente elas são diferentes.

No polimorfismo sempre se comportando diferente.
Porque no polimorfismo a operação do método é tão abstrata que não tem como prover um comportamento padrão, por exemplo, o slide citado acima referente aos pagamentos.

Já na sobrescrita pode ser ou não que o comportamento seja diferente.

No caso do slide acima referente ao saldo, existe um comportamento padrão que pode ser usado em alguns casos, mas se caso precisarmos de um comportamento diferente podemos utilizar também. Nesse caso a gente sobrescreve, usa o que está na classe mãe e acrescenta.

Há casos em que podemos sobrescrever 100%, provendo uma implementação completamente diferente da classe mãe sem problema algum. Mas caso queira e precisar, pode usar o que está na classe mãe também.

Existe um melhor? 

-Não. O uso dos dois é referente a sua necessidade, de acordo ao que a sua implementação pede e do que o contexto necessita. Cada um dos dois são muito bons na programação orientada a objetos. 




