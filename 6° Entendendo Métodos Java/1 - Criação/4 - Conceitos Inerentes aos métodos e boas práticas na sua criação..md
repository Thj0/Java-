
### Particularidades 

 - Assinatura: é a forma de identificar unicamente o método 
	 Ass = nome + parâmetros
	 
	 Método:
	 ``public double calcularTotalVenda (double precoItem1, double precoItem2, double precoItem3) {...}``
	 
	 Assinatura: 
	 `calcularTotalVenda (double precoItem1, double precoItem2, double precoItem3)`


Saber identificar uma assinatura de um método é importante para o conceito de sobrecarga.

___
 - Construtor e Destrutor: são métodos especiais usados na Orientação a Objetos.

 - Mensagem: é o ato de solicitar ao método que o mesmo execute. Esta pode ser direcionada a um objeto ou a uma classe.
___

 - Passagem de parâmetros: 
	 - Por valor (cópia)
	 - Por referência (endereço)

Por valor (cópia): 
```java
int i = 10;
public void fazerAlgo (int i) { 
	
	i = i + 10;
	System.out.println("Valor de i dentro :" + i);
	
}
System.out.println("Valor de i fora :" + i);
```

___
# Boas práticas

- Nomes devem ser descritivos, mas curtos 
- Notação camelo 

`verificarSaldo(); executarTransferencia(...); existeDebito();`

 - Deve possuir entre 80 e 120 linhas
 - Evite lista de parâmetros longas 
 - Visibilidade adequadas