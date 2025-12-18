# Anatomia das classes - 4° 



### Identação 

Basicamente **indentar** é um termo utilizado para escrever o código do programa de forma hierárquica, facilitando assim a visualização e o entendimento do programa 

Abaixo, veja um exemplo de algoritmo de validação de aprovação de estudante. Em uma aba, temos o mesmo código sem identação nenhuma, e na outra aba, temos o mesmo código seguindo um padrão de identação. Observe como é muito mais fácil entender a hierarquia do código na segunda aba.

____



public class BoletimEstudantil {

public static void main (String[] args){

int mediaFinal = 6;

if(media Final < 6)

System.out.println("REPROVADO.");

else if(mediaFinal == 6)

System.out.println("PROVA MINERVA");else 

System.ou.println("APROVADO.")

 }

}

____



public class BoletimEstudantil {

  public static void main (String[] args){

​    int mediaFinal = 6;

​    if(media Final < 6)

​      System.out.println("REPROVADO.");

​    else if(mediaFinal == 6)

​      System.out.println("PROVA MINERVA");

​    else 

​      System.ou.println("APROVADO.")

  }

}

_____



:exclamation:Todo código aplicado em cada uma das condições, está também identado em um bloco.





