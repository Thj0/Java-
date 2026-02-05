
 - Tipos de herança: 
 - Simples
 - Múltipla 
___
**Simples:**
 - A classe filha tem somente uma classe mãe:

![[Pasted image 20260204174329.png]]
___
**Múltipla:**
 - A classe filha tem uma ou mais classes mães:

![[Pasted image 20260204174439.png]]

A classe Estudante e Funcionário, são independentes.

Caso houvesse um atributo com o mesmo nome nas duas classes, teria um conflito de nomes.
Assim como métodos também.

Além de que não teria como saber se estaríamos utilizando os atributos/métodos de estudante ou funcionário.

___
Entretanto, nem toda linguagem tem herança múltipla.

 - Java - Não tem.
 - C# - Não tem.
 - Python - Tem.
 - C++ - Tem.

```Python

class A(B,C) :
	pass
```

___
Por quê Java e C# não tem herança múltipla?

Por conta de alguns problemas:
 - Diamante.
 - Conflito de nomes.
 
 
___
 Herança múltipla  (NÃO TEM em Java)

Uma classe herda de **duas ou mais classes ao mesmo tempo**.

       Pessoa
          ↑
     ─────┴─────
   Aluno             Funcionario
           ↑
	    Estagiario

Em pseudo-código ( não compila em Java):

`class Estagiario extends Aluno, Funcionario { }`

**Java NÃO permite herança múltipla de classes**