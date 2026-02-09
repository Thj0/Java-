
- Tipos: 
	- Estrutural
		- Composição: "Com parte Todo"
		- Ex: Pessoa e Endereço 

![[Pasted image 20260209120031.png]]

O "com parte todo" é a relação de existências entre instancias dos objetos, e isso mostra que 1 é composto pelo outro.

O "endereço" depende de "Pessoa" para existir, e é o que se chama da composição.

___
Código: 

```Java
class Pessoa { 
	Endereco endereco;
}
```

___
- Tipos: 
	- Estrutural
		- Agregação: "Sem Parte Todo"
		- Ex: Disciplina e Aluno

![[Pasted image 20260209120710.png]]

Agregação é o oposto da composição, ela é "Sem parte todo", ou seja, uma parte pode existir sem um todo.

Caso 'Disciplina' deixe de existir, 'Aluno', não pode deixar de existir, pois pode estar vinculado a outras disciplinas. 

Essa relação não é uma composição, é somente uma agregação onde um pode existir sem o outro.

___
Código:

```Java
class Disciplina { 
	Aluno aluno;
}
```

___
# Curiosidade

**Agregação x Composição**

Agregação - Se um deixar de existir, não necessariamente o outro deixa.
Em agregação essa relação de composição é mais fraca.


Composição - Se um deixar de existir, o outro deixa de existir também.

Definir conceitualmente qual desses 2 utilizar no meu código é bastante importante, para que eu consiga modelar de forma fidedigna a minha entidade do mundo real, a minha necessidade do mundo real. 

E além de tudo, referente a esses 2 conceitos, não existe um melhor ou pior, apenas aquele mais apropriado a minha necessidade momentânea. 

___
- Tipos: 
	- Comportamental
		- Dependência: "Depende de"

![[Pasted image 20260209122927.png]]

Dependência = (Uso temporário)

O método de dependência, é definidor por "Usar sem possuir", por assim dizer.

Dependência acontece quando uma classe usa outra de forma temporária, ou seja: ela precisa da outra para executar algo, mas não mantém um vínculo fixo com ela.
___
```Java 
class Compra { 
	...
	finalizar(Cupom cupom, ...)
	...
	}
}
```

Dependência é a relação mais fraca entre classes.
Uma classe só precisa da outra para executar uma ação.
___
**Como identificar uma dependência?**

Uma classe de outra quando ela: 

Usa a outra como parâmetro de método;
Cria o objeto apenas dentro de um método
Usa métodos da outra classe momentaneamente


Importante ressaltar que: 

Ela não guarda a outra classe como atributo.

___
# Curiosidade 

Herança x Associação 

Quem é melhor? Quando usar? 

Novamente, não existe um melhor nem pior, somente o mais apropriado para determinada situação e função.

Herança - É uma relação um pouco mais rígida, por que quando se faz uma herança, isso é definido durante o desenvolvimento, ou seja, se faz uma classe herdada de outra. E quando a aplicação começar a funcionar isso não vai mudar. 

Associação - É possível mudar esses valores durante a execução do meu software, pois ela vai estar nos meu atributos ou métodos. É mais flexível. 

___
Dica para utilizá-las:

Quando estiver em dúvida de como e onde usá-las, devo me perguntar;


Uma coisa É a outra? É um subtipo? 
Se for, utilizo herança.


Se não for utilizo associação.
Pois essa coisa vai USAR a outra.

___
Um erro comum é; onde utilizar uma associação, usar uma herança. Porque foi pensado em reuso, não em subtipos.

Então é muito importante saber diferenciar a relação de: 

É um.

Usa um.

Para saber quando utilizar associação ou herança. 


___

É UM        → Herança
USA         → Dependência
TEM UM      → Associação
   ↳ fraco  → Agregação
   ↳ forte  → Composição
Dependência = uso | Associação = estrutura


___
> **Dependência é sobre execução.  
> Associação (agregação/composição) é sobre significado.**

==Dependência não define estrutura — ela é consequência dela==
___
> **Dependência é ponto de partida para comportamento.  
> Associação é ponto de partida para estrutura.**

==Dependência modela “como o sistema funciona”; associação modela “o que o sistema é”.==
