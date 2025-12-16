# Métodos 

Todas as ações das aplicações são consideradas métodos.



Uma classe é definida por atributos e métodos.

Já vimos que atributos são, em sua grande maioria, variáveis de diferentes tipos e valores. Os métodos, por sua vez, correspondem a **funções ou sub-rotinas** disponíveis dentro das nossas classes.

____

#### Critérios de nomeação de Métodos 

Esses critérios não são obrigatórios, mas é recomendável que sejam seguidos, pois essas convenções facilitam a vida dos programadores ao trabalharem em códigos de forma colaborativa. Ao seguir estas convenções, tornamos o código mais legível para nós e também para outras pessoas. Para métodos, os critérios são: 



- Deve ser nomeado como verbo
- Seguir o padrão camelCase (Todas as letras minúsculas com a exceção da primeira letra da segunda palavra). 

____

Exemplos sugeridos para nomenclatura de métodos: 

```java
somar (int n1, int n2) {}

abrirConexão(){}

concluirProcessamento(){}

findById(int id){} // veremos muitos métodos em inglês

calcularImprimir(){} // há algo de errado nesse código, existe um conflito de RESPONSABILIDADE; Afinal a finalidade do método é, calcular ou imprimir?

//Seguindo as boas práticas um método contém apenas uma respondabilidade.

```

Se fosse para realizar as duas ações, teriamos que ter dois métodos correspondentes.

Um poderia chamar o outro e assim sucessivamente

____



:exclamation:Importante! Não existe em **Java** o conceito de **métodos** globais. Todos os métodos devem SEMPRE ser definidos dentro de uma classe.



____

### Critérios de definição de métodos 

Mas, como sabemos a melhor forma de definir os métodos das nossas classes? Para chegar à essa conclusão, somos auxiliados por uma convenção estrutural para todos os métodos. Essa convenção é determinada pelos aspectos abaixo:



1. **Qual a proposta principal do método?** 

Teremos que nos perguntar constantemente até compreender a real finalidade do mesmo.



2. **Qual o tipo de retorno esperado após executar o método?**

Devemos analisar se o método será responsável por retornar algum valor ou não.



:lantern: Caso o método não retorne valor nenhum, ele será representado pela palavra void.



1. **Quais os parâmetros serão necessários para execução do método?**

​	Os métodos as vexes precisam de argumentos como critérios para a execução.



2. **O método pssui o risco de apresentar alguma exceção:** 

   Exceções são comuns na execução de métodos, as vezes é necessário prever e tratar a possível existência de uma exceção.



3. **Qual a visibilidade do método?** 

​	Será necessário que o método seja viável a toda aplicação, somente em mesmo pacotes, através de herança somente a nível da própria classe.



____

Aqui temos um exemplo de uma classe com dois métodos e suas respectivas considerações:



```java
public class MyClass {
	
    public double somar(int num1, int num2){
        //LOGICA - FINALIDADE DO MÉTODO
        return ... ;
    }
    
    
  	public void imprimir(String texto){
        	// LOGICA - FINALIDADE DO MÉTODO
        	//AQUI NÃO PRECISA DO RETURN
        	//POIS NÃO SERÁ RETORNADO NENHUM RESULTADO
    }
    
    //throws Exception: indica que o método ao ser utilizado, pode gerar uma exceção.
    public double dividir(int dividendo, int divisor) throws Exception{
    }
    
    //Esse método não pode ser visto por outras classes no projeto.
    private void metodoPrivado(){
    }
    
    //Alguns equívocos estruturais 
    public void validar(){
    	//esse método deveria retornar algum valor 
    	//no caso boolean (true ou false)
    }
    
    public void calcularEnviar(){
        //um método deve representar uma única responsabilidade.
    }
    
    public void gravarCliente(String nome, String cpf, Intege){
        //esse método tem a finalidade de gravar informações de um cliente.
        //por que não criar um objeto cliente e passar como parâmetro?
        //veremos abaixo.
    }
    
    public void gravarCliente(Cliente Cliente) {
    }    
        //ou
    public void gravar(Cliente cliente){
    }
        
    }
}

```



