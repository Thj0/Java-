

```java 
/**  
 * Classe de exemplo para o exercício da Aula 1 de Operadores lógicos e relacionais, Controle de fluxo e Blocos. */

public class Main {  
  
    public static void main(String[] args) {  
  
        int i1 = 10;  
        int i2 = 20;  
        float f1 = 4.5f;  
        float f2 3.5f;  
        double d1 = 59.6d;  
        char c1 = 'x';  
        char c2 = 'y';  
        String s1 = 'Fulano';  
        String s2 = 'Beltrano';  
        String s3 = 'Sicrano';  
        boolean = true;  
        boolean = false;  
  
        long l1 = 1597L;  
        long l2 = 8997L;  
        byte y1 = 1;  
        short h1 = 25;  
  
        System.out.println("i1 == i2 " + (i1 == i2));  
        System.out.println("i1 != i2 " + (i1 != i2));  
        System.out.println("i1 > i2 " + (i1 > i2));  
        System.out.println("i1 <= i2 " + (i1 <= i2));  
  
  
        System.out.println("f1 == f2 " + ( f1 == f2));  
        System.out.println("f1 != f2 " + (f1 != f2));  
        System.out.println("f1 >= f2 " + (f1 >= f2));  
        System.out.println("f1 < f2 " + (f1 < f2));  
  
  
        System.out.println("c1 == c2 " + (c1 == c2));  
        System.out.println("c1 != c2 " + (c1 != c2));  
        System.out.println("c1 > c2 " + (c1 > c2));  
        System.out.println("c1 <= c2 " + (c1 <= c2));  
  
        
        System.out.println("s1 == s2 " + (s1 == s2));  
        System.out.println("s1 == s3 " + (s1 == s3));  
        System.out.println("s1 != s2 " + (s1 != s2));  
        
		// Aqui como são de similaridade e não de tamanho, é executável. */ 
        
        //System.out.println(s1 >= s2);  
        //System.out.println(s1 < s2);  
        
		/** 
		Em textos, não faz sentido aplicar operadores de tamanho. 

		Assim como dito, nem todo comparador seja ele relacional/tamanho ou de similaridade, eles podem ser aplicados a todos tipos de dados.
		*/
        
        System.out.println("b1 == b2 " + (b1 == b2));  
        System.out.println("b1 != b2 " + (b1 != b2));  

		/** Outro exemplo, os de similaridade são aplicados ou seja, dão certo,  já os de tamanho não.
		*/        
        
        //System.out.println(b1 > b2);  
        //System.out.println(b1 <= b2);  
        
		/** Novamente, não tem lógica perguntar se true é maior que false. Acabam se tornando operações inválidas.
		*/
        
        System.out.println("i2 > f1 " + (i2 > f1));  
        System.out.println("d1 == h1 " + (d1 == h1));  
        
        //System.out.println(s2 != c1);  
        //System.out.println(s3 != i1);  
		
			/** Outro tipo de situação, é que nem todo operador funciona com qualquer tipo de dado. 
		Além de que as operações apresentam tipos de dados diferentes.
		Mesmo usando o operador de similaridade, a aplicação se torna inválida.
		*/
		
		System.out.println("l1 == l2 " + (l1 == l2));  
        System.out.println("l2 >= l1 " + (l2 >= l1));  
        System.out.println("y1 != h1 " + (y1 != h1));
        
		/** Embora alguns tipos de dados sejam diferentes, é possível realizar operações desde que sejam do mesmo valor, seja numérico ou textos.
		Porém a partir do momento que os dados são muito diferentes, já não é possível, ocasionando em um erro de compilação.
		*/ 
        
	}   
}

``` 

