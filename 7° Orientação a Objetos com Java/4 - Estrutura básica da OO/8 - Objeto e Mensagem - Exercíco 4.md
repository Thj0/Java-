

Evolua o conceito do exercício 3 criando objetos da classe "Carro".

Use os métodos set/get, quando aplicáveis, para definir os valores dos atributos e exibir estes valores "get". Passe também uma mensagem para o cálculo do total pra encher o tanque.

Obs: Use a linguagem que gostar e siga as dicas sobre como criar métodos, atributos, etc. 

Obs: Use System.out, Console.WriteLine ou print.

```Java
public class RodarAplicação {

  

    public static void main(String[] args) { // Ponto de entrada para nossa aplicação iniciar

        Carro carro1 = new Carro();          

        /* Uma variável do tipo carro onde criamos um novo objeto, com um construtor que não possui parâmetros.

        O construtor é responsável por inicializar o objeto, e a variável carro1 passa a referenciar esse objeto na memória.

  

        Criamos um objeto vazio para depois acrescentar valor nele.

        */

  

        carro1.setCor("Azul");

        carro1.setModelo("Mercedes-Benz 450 SL");

        carro1.setCapacidadeTanque(47);

  

        System.out.println(carro1.getModelo());

        System.out.println(carro1.getCor());

        System.out.println(carro1.getCapacidadeTanque());

        System.out.println(carro1.totalTanque(6.19));

  
  
  

        Carro carro2 = new Carro("Vermelho", "Mercedez-Benz Classe C", 67);

        /*Objeto já criado com parâmetros, não vazio.

        Onde já passamos os valores dentro dos parâmetros criados pelos atributos do contrutor, utilizando sobrecarga.

        Os valores são passados para o contrutor, que os atribui aos atributos da classe.

        */

  

        System.out.println(carro2.getModelo());

        System.out.println(carro2.getCor());

        System.out.println(carro2.getCapacidadeTanque());

        System.out.println(carro2.totalTanque(6.19));

  

    }

}
```


___
Criamos objetos da classe Carro usando diferentes construtores, configuramos seus atributos com setters ou diretamente no construtor e utilizamos métodos para acessar dados e realizar cálculos.