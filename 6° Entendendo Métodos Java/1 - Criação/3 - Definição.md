
#### Padrão de definição:

**< ?visibilidade? > < ?tipo? > < ?modificador? > retorno nome (< ?parâmetros? >) < ?exceções? > corpo**

Vale ressaltar que, o que está com ponto de interrogação são opcionais. 
Já o 'retorno, nome e corpo, são obrigatórios'.

Pois são os itens mínimos pra gente definir um método.
Os outros são opcionais, de acordo com a necessidade podemos utilizá-los ou não.


### Onde: 

V: "public", "protected" ou "private" - Tem mais a ver com orientação a objetos.

T: concreto ou abstrato - Também sobre orientação a objetos.

M: "static" ou "final" - Orientação a objetos também.

R: "tipo de dado ou "void" - 
Qualquer um dos tipos primitivos de dados, ou um não primitivo também. Void é vazio, pode ser um método que não retorna nada.

N: nome que é fornecido ao método - 
Todas as regras que se aplicam a definição de variáveis, também se aplicam a criação de nome de métodos.

P: parâmetros que pode receber - Parâmetros que o método recebe.

E: exceções que pode lançar - Erros que pode explorar.

C: código que possui ou vazio - 

____

# Exemplos 


public String getNome() {...}  - Método que retorna um texto, sem parâmetros.

public double calcularTotalNota() {...} - 

public int verificarDistancia(int cordenada1, int cordenada2) {...} - Método com parâmetros, recebendo duas coordenadas do tipo inteiro(primitivo).

public abstract void executar(); - Método abstrato vazio, com um corpo vazio.

public void alterarFabricante(Fabricante fabricante) {...} - Método que recebe um objeto como parâmetro, uma entidade. Esse parâmetro é um tipo complexo, normalmente chamado de entidade(objeto).

public Relatorio gerarDadosAnaliticos(Cliente cliente, List< Compra > compras) {...} - Outro método exemplo que novamente mostra como passar mais de um parâmetro. E novamente utilizando um tipo de parâmetro complexo 

**public static R N(P) {...}**


____

# Utilização 


Passa-se uma mensagem através de uma classe ou objeto.

nome_da_classe.nome_do_método(); ou nome_da_classe.nome_do_método(...);

nome_do_objeto.nome_do_método(); ou nome_do_objeto.nome_do_método(...);


Math.random(); ou Math.sqrt(4); - 
(Math) é uma classe do Java que nos disponibiliza algumas facilidades matemáticas, tipo os métodos random(Gera números aleatórios) ou sqrt(Raíz Quadrada).



usuario.getEmail(); ou usuario.alterarEndereco(endereço) -


Por padrão na linguagem Java, os métodos começam em letra maiúscula e os objetos em letra minúsculas