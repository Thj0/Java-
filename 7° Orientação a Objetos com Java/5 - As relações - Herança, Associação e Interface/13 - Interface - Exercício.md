
Apenas para praticar crie uma interface chamada "OperaçãoMatematica". 

Crie também 4 métodos das operações básicas: soma, subtração, multiplicação e divisão.

Obs: Use a linguagem qu gostar e siga as dicas sobre como criar classes. Tente não implementar algum dos métodos e veja o que acontece.

___
```Java
package OperaçõesMatematicas;

  

/*Interface de exemplo para o exercício de Orientação a Objetos. */

  

public interface OperacaoMatematica {

    void soma(double operando1, double operando2);

  
  

    void subtracao(double operando1, double operando2);

  
  

    void multiplicacao(double operando1, double operando2);

  

    void divisao(double operando1, double operando2);

  

}
```

___

```Java
package OperaçõesMatematicas;

  

class Calculadora implements OperacaoMatematica {

  
  

    @Override

    public void soma(double operando1, double operando2)

    {

        System.out.println("Soma: " + operando1 + " + " + operando2);

    }

  

    @Override

    public void subtracao(double operando1, double operando2)

    {

        System.out.println("Subtração: " + (operando1 - operando2));

    }

  

    @Override

    public void multiplicacao(double operando1, double operando2)

    {

        System.out.println("Multiplicação de: " + operando1  *  operando2);

    }

    @Override

    public void divisao(double operando1, double operando2)

    {

        System.out.println("Divisão: " + operando1 / operando2);

    }

  

}
```

___