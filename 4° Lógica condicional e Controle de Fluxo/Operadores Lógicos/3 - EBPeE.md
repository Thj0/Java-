Exemplos, Boas práticas e Exercícios.

___
## Utilização 

Qual utilizar?

A depender da necessidade, e do tipo de decisão que quero tomar.

___
### Curiosidades

 - Operadores bitwise: &, |, ^, ~

	_bitwise”_ significa operar **bit a bit** sobre números inteiros.
	✔️ Bitwise - opera **bit a bit** em números inteiros
	✔️ Lógicos - operam sobre **booleanos**
	⚠️ `&` e `|` **dependem do contexto**

| Operador | Uso como bitwise      | Uso como lógico                |
| -------- | --------------------- | ------------------------------ |
| &        | Sim (bit de inteiros) | Sim (booleanos)                |
|          |                       |                                |
| ^        | Sim(XOR bitwise)      | Sim(XOR)lógicos                |
| &&       | ❌                     | Sim(lógico com curto-circuíto) |

`&` e `|` **podem ser bitwise ou lógicos**, dependendo do **tipo dos operandos**.

___

 - Operadores shift: ~, >>, >>>, <<

	O que eles fazem:
	
	Eles **deslocam os bits** de um número para a esquerda ou direita.
	`<<`, `>>`, `>>>` e `~` **não são operadores lógicos**


| Operador | O que faz                                           |
| -------- | --------------------------------------------------- |
| <<       | Desloca bits para a esquerda (preenche com 0 )      |
| >>       | Desloca para a direita preservando o sinal.         |
| >>>      | Desloca para a direita sem preservar o sinal.       |
| ~        | Inverte todos os bits (NÃO é shift, é bitwise NOT ) |

`~` **não é operador shift**, ele é um **operador bitwise de inversão**.


Os operadores `&` e `|` podem atuar como operadores bitwise ou lógicos, dependendo do tipo dos operandos. Já os operadores de shift e o operador `~` são exclusivamente bitwise e não lógicos.

____

Exemplos

boolean b1 = true; 
boolean b2 = false;
boolean b3 = true;
boolean b4 = false;


b1 && b2  = false
b1 && b3 = true
b2 | | b3 = true
b2 | | b4 = false
b1 ^ b3 = false
b4 ^ b1 = true
!b1 !b2 = b1 false, b2 true

(i1 > i2) | | (f2 < f1) = false
((i1 + i2) < (f2 - f1)) && true = false 

____

## Boas práticas 

 - Crie variáveis auxiliares para guardar resultados intermediários

(salarioMensal < mediaSalario) && (quantidadeDependentes >= mediaDependentes)

pode ser 

(salarioBaixo) && (muitosDependentes)

boolean receberAuxilio = (salarioBaixo) && (muitosDependentes)


Tendo um código simplificado, torna o entendimento mais fácil.

Um código longo e sem especificações dificulta não só o entendimento, mas como a manutenção.

____

## Exercício 

Criar um simples projeto e codificar os exemplos dos slides anteriores para compreender as operações lógicas. Utilize operandos e expressões. 


____