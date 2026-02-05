
1. Apresentar os conceitos que ajudam a criar entidades a partir de outras entidades.
	 - Herança;
	 - Associação;
	 - Interface
___
# Herança 

"É o relacionamento entre classes em que uma classe chamada de subclasse (classe filha, classe derivada) é uma extensão, um subtipo, de outra classe chamada de superclasse (classe pai, classe mãe, classe base). Devido a isto, a subclasse consegue reaproveitar os atributos e métodos dela. Além dos que venham a ser herdados, a subclasse pode definir seus próprios membros. "

A principal finalidade da herança é criar subtipos.

É muito comum programadores acharem que, herança serve somente para reuso, porém essa não é sua finalidade.

O reuso na herança é uma consequência do seu uso, não o porquê de sua existência.

Podemos até ter reuso sem herança.

A herança é para criar subtipos, tipos mais específicos, mais especializados a partir de um tipo pré-existentes. 

Membros é só um termo que representa atributos e métodos.

___
 - **Códigos:**

```Java
class A extends B {

}
```

```C#
class A : B { 

}
```

```Python
class A(B):
	...
	
```

___
Exercitando


Crie a classe "Veículo", "Carro", "Moto" e "Caminhão".

Obs: Use a linguagem que gostar e siga as dicas sobre como criar classes. Faça a relação de herança que julgue adequada. 

