
# Argumentos 


Quando executamos uma classe que contenha o método main, o mesmo perimite que passamos um array [ ] de argumentos do tipo String. Logo podemos após a definição da classe a ser executada informar estes parâmetros, exemplo: 

1. java MinhaClasse argumentoUm, argumentoDois 


Exemplo

```
public class AboutMe { 
	public static void main(String[] args){
		//Os argumentos começam com índice 0.
		
		String nome = args [0];
		String sobrenome = args [1];
		
		int idade = Integer.valueOf(args[2];)
		double altura = Double.valueOf(args[3]);
		
		System.out.println("Olá, me chamo " + nome + sobrenome);
		System.out.println("Tenho " + idade + anos ");
		System.out.println("Minha altura é " + altura + "cm"); 
	}
}
```

___
Exemplo corrigido, pois pelo terminal identifiquei um bug;

```
public class AboutMe { 
	public static void main(String[] args){
		//Os argumentos começam com índice 0.
		
		String nome = args [0];
		String sobrenome = args [1];
		
		int idade = Integer.valueOf(args[2];)
		double altura = Double.valueOf(args[3]);
		
		System.out.println("Olá, me chamo " + nome + " " + sobrenome);
		System.out.println("Tenho " + idade + anos ");
		System.out.println("Minha altura é " + altura + "cm"); 
	}
}
```

Ao receber a execução pelo terminal, eu não estava entendendo o porque dos parâmetros 'nome' e 'sobrenome', estarem sendo impressos colados.

'JhonataAndrade' - Desse forma.

Depois de muito quebra cabeça entendi que estavam sendo concatenados juntos, mas não sabia o por que de jeito algum. 

Então decidi pedir ajuda ao ChatGPT.

Perguntei - "Estou estudando, e na aula executamos um código pelo terminal para ter uma noção de cliente. Porém, quando executo, meu nome e sobrenome saem colados. Vou te mandar o código e quero que me auxilie na correção desse bug."

Como era somente o nome e sobrenome, resolvi apenas mandar a primeira linha do código de saída.

`System.out.println("Olá, me chamo " + nome + sobrenome);`


Então ao enviar a linha do código que 'supostamente' estava errada, ele me informou o porque do problema.

A resposta seguinte foi: 

"Você está **concatenando duas Strings sem nenhum separador entre elas**."
O Java **não adiciona espaços automaticamente**.


___

Perguntei - Por que a necessidade de um separador, hoje em dia? Na aula, o código do professor está do mesmo jeito, porém no terminal dele todas as informações foram impressas com perfeição. Pela data do computador dele a aula foi gravada em 2022.

E resumidamente a resposta foi:

## 1️⃣ Por que **sempre** é necessário um separador?

Porque **String não tem semântica**, só conteúdo.

Para o Java:

`nome + sobrenome`

significa **apenas**:

> “pegue os caracteres de `nome` e cole imediatamente com os de `sobrenome`”

O Java **não sabe** que isso representa:

- nome próprio
    
- sobrenome
    
- palavras distintas
    
- linguagem humana
    

Então:

`"Jhonata" + "Alves" = "JhonataAlves"`

Isso **nunca mudou**, não muda hoje e **não mudou em 2022**.

👉 **Não existe versão do Java que adicione espaço automaticamente.**

___
## 2️⃣ Então por que no terminal do professor funcionou?

Aqui está o ponto-chave 👇  
**Não foi o Java que fez diferente — foi a entrada de dados.**

O mais provável é que **uma dessas situações** tenha ocorrido na aula:

---

### 🔹 Possibilidade 1 — O espaço já veio no argumento

O professor pode ter executado assim:

`java AboutMe "Jhonata Alves" 25 1.75`

Nesse caso:

`args[0] = "Jhonata Alves" args[1] = "25"`

Ou então:

`java AboutMe Jhonata "Alves Silva" 25 1.75`

👉 **O espaço já estava dentro da String**, então não parecia haver problema.

---

### 🔹 Possibilidade 2 — Ele digitou o espaço sem perceber

Exemplo:

`java AboutMe "Jhonata " Alves 25 1.75`

Note o espaço **dentro das aspas** após o nome.

Resultado:

`Jhonata Alves`

Mas isso é **ilusão de funcionamento**, não regra.


____

## 3️⃣ O Java mudou de 2022 pra cá?

❌ **Não nesse ponto.**

- Concatenação de `String` funciona do **mesmo jeito há mais de 20 anos**
    
- Java 8, 11, 17, 21… todos se comportam igual aqui
    

Se isso tivesse mudado, **milhões de sistemas quebrariam**.

---
# 4️⃣ A regra de ouro (guarde isso)

> **O programador é responsável pela formatação da saída.**

Se você quer:

`Nome Sobrenome`

Você **tem que escrever isso explicitamente**:

`nome + " " + sobrenome`

Ou:

`"%s %s"`

Ou:

`String.join(" ", nome, sobrenome);`

---
# 5️⃣ Conclusão direta

- ✅ Seu código está certo
    
- ❌ O comportamento não mudou
    
- 🎥 A aula de 2022 provavelmente:
    
    - usou aspas no terminal
        
    - ou já tinha espaço embutido
        
    - ou o detalhe passou despercebido
        

Você **aprendeu do jeito correto**, não do jeito “ilusório”.
____

Na segunda explicação ele me deu algumas possibilidades do que poderia ter acontecido, mas não foi o caso. Após eu retroceder a minutagem da aula, percebi o que de fato era:

O uso de " " aspas, servindo de fato como um separador.

No primeiro exemplo o código de saída, na IDE, não tem aspas para representar o espaço no terminal após 'nome + ', porém como eu estou escrevendo tudo, passou despercebido por mim.

O meu estava assim: `System.out.println("Olá, me chamo " + nome + sobrenome);`

E quando eu retrocedi a minutagem na vídeoaula, no código do professor tinha.

Estava assim: `System.out.println("Olá, me chamo " + nome + " " + sobrenome);`

____
# Conclusão

Esse meu "erro" e um pouco de falta de atenção, me ajudaram a aprender uma coisa nova, pois de forma alguma me lembrava de ter aprendido sobre a "declaração" do separador (o uso de aspas).
E ainda aprendi mais um pouco sobre como o Java entende a concatenação.