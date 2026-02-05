
Crie as classes "Funcionário", "Gerente", "Vendedor" e "Faxineiro".

Realize upcasts e downcasts.

Obs: Use a linguagem que gostar e siga as dicas sobre como criar classes. Faça a relação de herança de acordo com o slide.
___
Analise do comportamento de Polimorfismo e Sobrescrita.
___ 

```Java
public class Funcionario {


}
```

___
```Java
//Substipo da classe Funcionario.
class Faxineiro extends Funcionario {


}
```

___
```Java
//Substipo da classe Funcionario.
class Vendedor extends Funcionario { 


}
```

___
```Java 
//Substipo da classe Funcionario.
class Gerente extends Funcionario {


}
```

___
```Java 
class RodarAplicação {

	public static void main(String[] args) {

        Funcionario funcionario = new Funcionario();

  

        Funcionario gerente = new Gerente();

        Funcionario vendedor = new Vendedor();

        Funcionario faxineiro = new Faxineiro();

  

        //Gerente gerente_ = new Funcionario();

        Vendedor vendedor_ = (vendedor) new Funcionario();

  

	}	
}


```