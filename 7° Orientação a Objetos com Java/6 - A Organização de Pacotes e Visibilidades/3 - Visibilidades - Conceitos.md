
Também são chamadas de: "Modificadores de acesso".


"Um modificador de acesso tem como finalidade determinar até que ponto uma classe, atributo ou método pode ser usado. A utilização de modificadores de acesso é fundamental para o uso efetivo da Orientação a Objetos. Algumas boas práticas e conceitos só são atingidos com o uso coreto deles."


 - Tipos: 
	 - Private
	 - Protected
	 - Public

___
Em Python não é trabalhada essa ideia de visibilidades, em python tudo é 'public'.

___
Tipo: 
 
# Private: Só dentro da classe


```Java
private 

private int i; // Esse atributo só será visível dentro da classe em que foi criado

private void do(); /* Esse método também só sera visível dentro da classe em que foi criada. */
```

```C#
private 

private int i;
private void Do();
```

Por que usar? 

Encapsulamento total - É a base da segurança na programação. Você esconde a lógica interna para que ninguém altere o estado do objeto de forma indevida.

Facilidade de Manutenção - Como eu sei que ninguém de fora usa aquele método privado, eu posso alterá-lo ou deletá-lo sem medo de quebrar o resto do sistema.

Controle de Acesso - Você obriga o uso de métodos `public` (Getter e Setter) para validar qualquer mudança de dados.
___
Tipo: 

# Protected: Dentro da classe, mesmo pacote e subclasses


```Java
protected 

protected int i;
protected void Do();
```

```C#
protected 

protected int i;
protected void Do();
```

Por que usar? 

Para proteger do mundo externo (como se fosse private), mas não bloqueia seus herdeiros de expandir a funcionalidade.

Além de permitir que quem possui sua classe possa personalizar comportamentos internos sem precisar "quebrar" a  segurança do objeto.

___
Tipo:

# Public: Em qualquer lugar


```Java 
public 

public int i; // Esse atributo é visível em qualquer lugar.

public void do(); // Esse método é visível em qualquer lugar.
```

```C# 
public 

public int i;
public void Do();
```

Quando usar?

Para métodos que definem as ações principais do objeto (ex: `carro.acelerar()`)

Constantes - Valores que nunca mudam e são úteis para todos

API: Tudo o que eu quero que os outros desenvolvedores utilizem livremente ao usar sua biblioteca.

# O Risco do Excesso

Diferente do `protected`, usar `public` em **atributos** (variáveis) é geralmente considerado uma má prática. Isso porque qualquer um pode alterar o valor sem validação, quebrando o encapsulamento.

**Dica de Ouro:** O ideal é manter os atributos `private` ou `protected` e usar métodos `public` (Getters e Setters) para controlá-los.

___
# CURIOSIDADE

Qual usar?! 

Cada visibilidade tem sua finalidade.


Para proteção de dados ou atributos - `private`

Para o funcionamento da aplicação e a facilidade de comunicação - `public` ou `protected`

Por fim, é de fácil percepção que durante a execução e da necessidade do software, usaremos todos os tipos de visibilidade, claro que, dependendo da necessidade.
___