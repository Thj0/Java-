
```Java
/**

 * Classe de exemplo para o exercício da Aula 2de Operadores lógicos e relacionais, Controle de fluxo e Blocos.

 */

public class ExDois {

  

    public static void main(String[] args) {

        boolean b1 = true;

        boolean b2 = false;

        boolean b3 = true;

        boolean b4 = false;

        System.out.println("b1 && b2 " + (b1 && b2)); // false

        System.out.println("b1 && b3 " + (b1 && b3)); // true

  

        System.out.println("b2 || b3 " + (b2 || b3)); // true

        System.out.println("b2 || b4 " + (b2 || b4)); // false

  
  

        System.out.println("b1 ^ b3" + (b1 ^ b3)); // false

        System.out.println("b4 ^ b1" + (b4 ^ b1)); // true

  
  

        System.out.println(!b1); // false

        System.out.println(!b2); // true

        System.out.println(!b3); // false

        System.out.println(!b4); // true

  
  

        int i1 = 10;

        int i2 = 5;

        float f1 = 20f;

        float f2 = 50f;

  

        System.out.println("((i1 + i2) < (f2 - f1)) && true " + (((i1 + i2) < (f2 - f1)) && true)); // true

        System.out.println("(i1 > i2) || (f2 < f1) " + ((i1 > i2) || (f2 < f1))); // true

  
  

        double salarioMensal = 13013.13d;

        double mediaSalario = 10500d;  

        int quantidadeDependentes = 4;

        int mediaDependentes = 2;

  

        System.out.println((salarioMensal < mediaSalario) && (quantidadeDependentes >= mediaDependentes)); // false

  

        boolean salarioBaixo = salarioMensal < mediaSalario;

        boolean muitosDependentes = quantidadeDependentes >= mediaDependentes;

  

        System.out.println((salarioBaixo) && (muitosDependentes)); // false

  

        boolean recebeAuxilio = (salarioBaixo) && (muitosDependentes);

        System.out.println("Apto a receber o auxílio." + recebeAuxilio); // false

  
  

    }

}

```

____
