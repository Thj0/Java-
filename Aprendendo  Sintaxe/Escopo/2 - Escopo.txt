# Escopo 

Escopo pode ser entendido como o ambiente onde uma variável pode ser acessada. Em Java, o escopo de variáveis **vai de acordo com o bloco onde ela foi declarada.**

A variável é criada no primeiro acesso à ela, se tornando inacessível após o interpretador sair do bloco de execução ao qual ela pertence. Portanto, esta variável não pode ser ligada ou manipulada por rotinas e códigos que estão fora do seu bloco de declaração, ou seja, fora do escopo da variável.

Em uma Classe, podemos visualizar a diferença de escopos. Os atributos (variáveis) são declarados no corpo principal da Classe, sendo portanto acessíveis por todos os métodos.

Caso você declare uma variável DENTRO DE UM MÉTODO, o escopo dessa variável está limitado apenas ao corpo desse método, ou seja, dentro das chaves que limitam o método.

Uma parte fundamental na elaboração de algoritmos simples ou complexos é determinar a localização do código em questão. Sem um domínio sobre escopo de códigos seu projeto tende a conter falhas estruturais e comprometer a proposta principal da aplicação.



```java
public class conta() {
    //variavel da classe conta
    double Saldo = 10.0

	public void sacar(Double valor){
    		//variável local do método
    		double novoSaldo = saldo - valor;
    }
    public void imprimirSaldo(){
        	//disponpivel em toda classe
        	System.out.println(saldo);
        	//somente o método sacar conhece esta variável 
        	System.out.println(novoSaldo);
    }
    public double calcularDividaExponencial(){
        //variável local de método 
        double valorParcela = 50.0;
        double valorMontante = 0.0; // comaçando a variável 
        for(int x = 1; x <= 5; x++){//x variável de escopo local do laço for
            //esta variavel será reiniciada a cada execução
            double valorCalculado = valorParcela * x;
            valorMontante = valorMontante + valorCalculado;
           
    }
    
    //escopo de fluxo
    //fora do escopo do for:
    //x e valorCalculado nunca estarão disponíveis 
    
    return valorMontante;
}
```







:traffic_light:

É  importante ter a capacidade de interpretar fronteiras do nosso código.