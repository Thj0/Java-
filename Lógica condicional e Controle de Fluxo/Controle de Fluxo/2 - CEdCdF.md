### Criando estruturas de Controle de Fluxo

___

## Criação 

**Tipos:
 - Decisão: Estrutura que avalia uma condição booleana ou variável para direcionar o fluxo de execução.

 - Opção: if (se), switch (escolha) e operador ternário.

____

**Tipo
  - Decisão: if, if-else, if-else-if, if-else-if-else

![[Pasted image 20251222180500.png]]

Em Java;

Exemplo:
```Java 
if (idade > 18) {

}


if (aprovado) {

} else {

}


if (casada&&temFilhos) { 

} else if (casada&&semFilhos) { 

} else { 

}
```


____
**Tipo

 - Decisão: Operador Ternário

![[Pasted image 20251222181712.png]]

Em Java;

Exemplo:
```Java

Condição ? true : false;

ligado ? desligar : ligar;

Condição ? true : null; 

emMovimento ? freia : null; 
 
```


___

**Tipo: 

 - Decisão

![[Captura de tela 2025-12-22 182507.png]]


Em Java;

Exemplo: 
```Java

switch (olhos) {

case "Azuis":
break;

case "Verdes":
break;

case "castanhos"
break;

default: 

break;
}
```