

```Java
public class ClasseMae { 

    void metodo1() {
    
        System.out.println("Método 1 da Classe Mãe");
        
    }

    void metodo2() {
    
        System.out.println("Método 2 da Classe Mãe");

    }

}
```

```Java
class ClasseFilha1 extends ClasseMae {

    @Override

    void metodo1() {
    
        System.out.println("Método 1 da Classe Filha 1");
        
    }

}
```

```Java
class ClasseFilha2 extends ClasseMae {

    @Override

    void metodo1 () {
    
        System.out.println("Método 1 da Classe Filha 2");

    }

    @Override

    void metodo2 () {

        System.out.println("Método 2 da Classe Filha 2");

    }

}
```

```Java
class RodarAplicacao {

    public static void main(String[] args) {

        ClasseMae[] classes = new ClasseMae[]{

            new ClasseFilha1(),

            new ClasseFilha2(),

            new ClasseMae()};

  
        for (ClasseMae classe: classes) {

            classe.metodo1();
        }

        System.out.println("");

        for (ClasseMae classe: classes) {

            classe.metodo2();
        }

        System.out.println("");

  
        ClasseFilha2 classeFilha2 = new ClasseFilha2();

        classeFilha2.metodo2();

    }
}
```

1 - O que o código está demonstrando? 

Polimorfismo + sobrescrita de métodos (@Override)
Ou seja: o mesmo método se comportando de formas diferentes, dependendo do objeto real.

___
2 - O primeiro trecho é o coração do exemplo

```Java
ClasseMae[] classes = new ClasseMae[]{
    new ClasseFilha1(),
    new ClasseFilha2(),
    new ClasseMae()
};
```

Ali acontece algo importante: 

 - O tida da variável é `ClassMae`
 - Mas os objetos reais são: 
	 - `ClasseFilha1`
	 - `ClasseFilha2`
	 - `ClasseMae`

Isso é polimorfismo:

Uma classe mãe referenciando objetos de classes filhas 

___
3 - O primeiro `for` é uma chamada para o `metodo1()`

```Java
for (ClasseMae classe: classes) { 
    classe.metodo1();
}
```

O que acontece ali? 

 - O Java não olha o tipo da variável (`ClasseMae`)
 - Ele olha qual é o objeto de verdade em memória

Então: 

 - Se `ClasseFilha1` sobrescreveu `metodo1()` - chama o da filha

 - Se `ClasseFilha2` sobrescreveu `metodo1()` - chama o da filha

 - Se for `ClasseMae` - chama o da mãe


Isso se chama ligação dinâmica (dynamic dispatch)

___
4 - O segundo `for` é uma chamada do `metodo2()`

```Java
for (ClasseMae classe: classes) { 
    classe.metodo2();
}
```

Ali vale a mesma regra: 

Se a filha sobrescreveu `metodo2()`, o Java chama o método da filha

Se não sobrescreveu, ele usa o método herdado da classe mãe.

Ou seja: 

O comportamento depende de quem implementou o método.

___
5 - O trecho final é bastante importante

```Java 
ClasseFilha2 classeFilha2 = new ClasseFilha2();
classeFilha2.metodo2();
```

Aqui não tem polimorfismo: 

A variável é do tipo `ClasseFilha2`
O objeto também é `ClasseFilha2`

Então o Java chama diretamente o `metodo2()` da `ClasseFilha2`.
___
# Curiosidade

1. O tipo da variável não define qual método será executado.

2. Quem define é o objeto real.

3. Isso só funciona para métodos sobrescritos

4. É assim que o Java implementa polimorfismo.