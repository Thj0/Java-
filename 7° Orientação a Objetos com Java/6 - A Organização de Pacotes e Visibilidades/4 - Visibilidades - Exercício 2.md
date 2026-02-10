
Ver projeto de exemplo para entender o funcionamento.

```Java
package one.digitalinnovation.oo

public class Classe1 { 
	
	private String atributo1; //É visto somente dentro da classe.
	
	protected String atributo2; //Dentro da classe/subclasse e mesmo pacote.
	
	public String atributo3; //Em qualquer lugar.
	
	
	
	private void metodo1() {
	
	}
	
	protected void metodo2() {
	
	}
	
	public void metodo3() {
	
	}
}
```

```Java
package one.digitalinnovation.oo

class Classe2 extends Classe1 {
	
	//Atributos próprios
	
	void metodo() {
	
		//Atributo2 e 3
	
	}
	
	//metodo2 e 3
}
```

```Java
package one.digitalinnovation.oo

class Classe3 { 
	
	Classe1 classe1;
	
	void metodo() { 
	
		//atributo2 e 3
		
		//metodo2 e 3
	
	}
}
```

atributo1 - private.
pertence somente a classe1


___
```Java
package outro.pacote;

import one.digitalinnovation.oo.Classe1;

class Classe4 { 
	
	Classe1 classe1;
	
	void medoto() {
	
	//atributo3
	classe1.atributo3 // Somente ele é public
	//metodo3
	
	}
	
}
```

atributo1 - private.
metodo1 - private.
pertence somente a classe1


atributo2 - protected.
metodo2 - protected.
pertence somente ao pacote - one.digitalinnovation.oo


E essa ideia acompanha aos métodos, somente é visível o metodo3( ).
___