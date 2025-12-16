# Exercitando

Nessa atividade foi criado um exemplo de uma classe para representar uma SmartTv onde:

1. Ela tenha as características: ligada (boolean), canal (int) e volume (int)
2. Nossa TV poderá ligar e desligar e assim mudar o estado ligada
3. Nossa TV aumentará e diminuirá o volume sempre sem +1 ou -1
4. Nossa TV poderá mudar de canal de 1 em 1 ou definindo o número correspondente

[ Exercício ](https://github.com/Thj0/DIO-Basic-Java-/tree/main/EX-smart-tv)

De início 

Criamos a Classe SmartTv com a extensão .java

e iniciamos o Projeto com nossos atributos para ter interação de estados

```java
//1.Ela tenha as características: ligada (boolean), canal (int) e volume (int)

boolean ligada = false;
int canal = 1;
int volume = 13;
```

____



Feito isso, renomeamos nossa classe "App" para "Usuário"  para que o projeto se tornasse mais intuitivo.

 e dentro do nosso método main/Console/Exibição:

```java
SmartTv smartTv = new SmartTv
//Essa é uma forma de criar uma classe para ilustrar a interação dos métodos e atributos e etc...
    
//Estado atual    
System.out.println("TV Ligada?" + smartTv.ligada);
System.out.println("Canal Atual :" + SmartTv.canal);
System.out.println("Volume atual :" + SmartTv.volume);
```

____



Voltando para nossa classe

Vamos criar os métodos que manipulam esses estados, por assim dizer:

```java
//2.Nossa TV poderá ligar e desligar e assim mudar o estado ligada
public void ligar(){
    ligada = true;
}

public void desligar() {
    ligada = false;
}
```

____



Após isso vamos voltar para a interface de Usuário;

Onde chamaremos o método 'ligar'

```java
//Declarando novos status
smartTv.ligar ();
System.out.println("A Tv continua ligada?" + smartTv.ligada);

smartTv.desligar();
System.out.println("E agora, ainda está ligada?" + smartTv.ligada);
```

E com isso vamos executando nossa aplicação, para checar se o nosso algoritmo está sendo bem estruturado para nos dar as informações desejadas.

_____



Seguindo o projeto e,

retornando a classe SmartTv, criaremos outros métodos para os requisitos citados acima:

```java
//3.Nossa TV aumentará e diminuirá o volume sempre sem +1 ou -1
//Será parecido com o método ligar e desligar

public void aumentarVolume () {
    volume++;
    //volume = volume +1;
}

public void diminuirVolume (){
    volume--;
    //volume = volume -1;
}
```

____



Voltando a nossa main:

```
//Entendemos que o volume atual é 13
//Porém apertei para diminuir o volume 3x e aumentei 1x


	smartTv.dimunuirVolume();
    smartTv.dimunuirVolume()
    smartTv.dimunuirVolume();
    smartTv.aumentarVolume();
 	System.out.println("Volume atual :" + smartTv.volume);

//Queremos que o sistema imprima essa mensagem
//Assim quando ela for ligada, iniciará no volume 11
```

____



Na classe SmarTv:

```java
//acionando o método aumentarVolume
System.out.println("Aumentando o volume para: " + volume);
//será exibida essa mensagem

//e com o método diminuirVolume
System.out.println("Diminuindo o voluma para : " + volume);
//essa será a mensagem exibida
```

_____



Novamente na classe Usuário:

Checamos a funcionalidade dos dois códigos, entendendo que são duas etapas 

A televisão, que é um objeto;

e um Usuário interagindo sobre aquele objeto.

Com tudo certo, avaliamos que de fato estava tendo consistência.



____

Na classe SmartTv.

Criaremos o ultimo requisito do exercício:

```java
//4.Nossa TV poderá mudar de canal de 1 em 1 ou definindo o número correspondente
//O método utilizado é bem parecido com o de volume, seguindo a mesma lógica.



public void canalPosterior () {
    canal++;
    //canal = canal +1; 
}

public void canalAnterior () {
    canal--;
    //canal = canal -1;
}


//Porém para que esses dois métodos acima funcionassem, seria necessário a criação de outro método, o de mudar o canal.
//Contendo um parâmetro
//Com isso estamos disponibilizando para o Usuário que el informe o número do canal desejado.
//Então é de suma importância o parâmetro criado.

public void mudarCanal(int novoCanal){
    canal = novoCanal;
}
```

____



Na classe Usuário 

```java
//criamos um código para chamar o método criado 

smartTv.mudarCanal(17) - // o "17" significa o canal escolhido.
System.out.println("Canal Atual : " + smartTv.canal);

//Sendo assim, imprimimos antes e depois.
//e com isso checamos as duas funcionalidades, tanto a anterior criada, como essa atual.
//Para podermos ver, se conseguimos ter uma boa implementação
```

____



***APRENDIZADO*** 

- O Nome do métodos são legíveis;
- Nem todos os métodos, precisam me dar algum retorno;
- Alguns métodos vão ter parâmetros;
- E esses métodos podem manipular as variáveis/características do nosso objeto principal.