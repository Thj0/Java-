
# Objetivos 

1. Entender como funcionam.

# Relembrando

 - É uma instrução de interrupção;
 - Simbologia: return.

____
# Funcionamento.

O método executa seu retorno quando: 

 - Completa todas suas instruções internas;
 - Chega a uma declaração explícita de retorno;
 - Lança uma exceção.

___
# Considerações.

 - O tipo de retorno do método é definido na sua criação e pode ser um tipo primitivo ou objeto;
 - O tipo de dado do retorno deve ser compatível com o do método;
 - Se o método for sem retorno(void), pode ou não ter um "return" para encerrar sua execução.

___

## Exemplos 

	public String getMensagem() {
	return "Ola!";
	}

	public double getJuros() {
	retunr 2.36;
	}

	public int getParcelas() {  
	return 1.36f;
	}
	// um inteiro não retorna um double.


	public void setIdade() { 
		return 10;
	}

	public void executar() {
		...
		return;
		...
		
	}

___

# Exercitando 

Recrie a aplicação que calcula a área dos 3 quadriláteros notáveis. Agora faça os métodos retornarem valores.