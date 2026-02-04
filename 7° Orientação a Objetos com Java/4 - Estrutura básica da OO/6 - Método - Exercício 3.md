
Evolua o conceito do exercício 2 e defina 1 método para calcular o valor total para encher o tanque. Este deve receber como parâmetro o valor da gasolina. Faça também duas sobrecargas do construtor.

Obs: Siga as dicas sobre como criar métodos.

Obs: Crie métodos específicos para fornecer e obter os valores dos atributos (set/get), caso aplicável.
___

```Java
public class Carro {

  

    String cor;

    String modelo;

    int capacidadeTanque;

  

    // Construtor aqui

    Carro() {

  

    }

  

    Carro (String cor, String modelo, int capacidadeTanque) {

        this.cor = cor;

        this.modelo = modelo;

        this.capacidadeTanque = capacidadeTanque;

    }

  

    void setCor (String cor){

  

        this.cor = cor;

    }

  

    String getCor() {

  

        return cor;

    }

  

    void setModelo(String modelo) {

  

        this.modelo = modelo;

    }

  

    String getModelo() {

  

        return modelo;

    }

  

    void setCapacidadeTanque(int capacidadeTanque) {

        this.capacidadeTanque = capacidadeTanque;

    }

  

    int getCapacidadeTanque() {

  

        return capacidadeTanque;

    }

  

    double totalTanque(double valorCombustivel) {

  

        return capacidadeTanque * valorCombustivel;

  

    }

}

```


Em OO, uma boa prática é proteger os atributos da classe usando private.

Mas ai surge o problema:
	Como acessar o u alterar esses valores fora da classe?

É aí que entram:

- get - pegar/ler o valor
- set - alterar/modificar o valor

Eles fazem parte do encapsulamento.
___
Sobre o `this`

this faz referência ao objeto atual.

 - O atributo da classe recebe o valor passado por parâmetro.
 - Evita conflito de nomes.

___
