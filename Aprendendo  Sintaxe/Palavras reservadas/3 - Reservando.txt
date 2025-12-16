# Escopos de uso 



:monkey: Observação importante.

Java possui 52 Palavras reservadas oficiais (keywords).

***true***, ***false***, e ***null*** não são palavras reservadas, são literais.

***



1. Estrutura do código (organização do projeto).

| Uso                    | Palavras      | Obersvação                                      |
| ---------------------- | ------------- | ----------------------------------------------- |
| Organização de pacotes | **package**   | Define a qual pacote a classe pertence.         |
| Importação de classes  | **import**    | Permite usar classes de outros pacotes.         |
| Definição de classe    | **class**     | Cria uma classe.                                |
| Interface              | **interface** | Define um contrato (métodos sem implementação). |
| Enumeração             | **enum**      | Define um conjunto fixo de constantes.          |



____

2. Modificadores de acesso (escopo de visibilidade).

| Uso                        | Palavras      | Observação                                                   |
| -------------------------- | ------------- | ------------------------------------------------------------ |
| Acesso total               | **public**    | Visível por qualquer classe.                                 |
| Acesso restrito à classe   | **private**   | Visível somente dentro da própria classe.                    |
| Acesso por pacote /herança | **protected** | Mesmo pacote ou subclasses.                                  |
| Acesso padrão              | (**default**) | Não é palavra reservada, ocorre quando não se usa modificador. |



____

3. Modificadores de comportamento.

| Uso                 | Palavras       | Observação                                     |
| ------------------- | -------------- | ---------------------------------------------- |
| Constante           | **final**      | Não pode ser alterado, herdado ou sobrescrito. |
| Método de classe    | **static**     | Pertence à classe, não ao objeto.              |
| Classe abstrata     | **abstract**   | Não pode ser instanciada.                      |
| Classe imutável     | **sealed**     | Restringe quem pode herdar.                    |
| Permite herança     | **non-sealed** | Libera herança de classe sealed.               |
| Controle de herança | **permits**    | Define quais classes podem herdar.             |



____

4. Tipos primitivos (escopo de dados).

| Uso             | Palavras    | Observação                    |
| --------------- | ----------- | ----------------------------- |
| Booleano        | **boolean** | **true** ou **false**.        |
| Inteiro         | **byte**    | -128 a 127.                   |
| Caractere       | **char**    | Um caractere Unicode.         |
| Inteiro curto   | **short **  | Menor que **int**.            |
| Inteiro padrão  | **int**     | Tipo inteiro mais usado.      |
| Inteiro longo   | **long**    | Valores grandes.              |
| Decimal simples | **float**   | Menor precisão.               |
| Decimal preciso | **double ** | Mais usado para decimais.     |
| Classe base     | **void**    | Indica que não retorna valor. |



_____

5. Controle de fluxo (escopo de execução).

| Uso              | Palavras     | Observação                               |
| ---------------- | ------------ | ---------------------------------------- |
| Condicional      | **if**       | Executa se a condição for verdadeira.    |
| Alternativa      | **else**     | Executa se o **if** for falso.           |
| Escolha múltipla | **switch**   | Avalia múltiplos casos.                  |
| Caso específico  | **case**     | Opção dentro do **switch**.              |
| padrão           | **default**  | Executa se nenhum **case** for atendido. |
| Laço condicional | **while**    | Repete enquanto condição for verdadeira. |
| Laço garantido   | **do**       | Executa ao menos uma vez.                |
| Laço contador    | **for**      | Loop com controle explícito.             |
| Interrupção      | **break**    | Sai de loop ou switch.                   |
| Continuação      | **continue** | Pula para próxima iteração.              |
| Retorno          | **return**   | Retorna valor ou encerra método.         |



_____

6. Tratamento de exceções (escopo de erro).

| Uso                | Palavras    | Observação                     |
| ------------------ | ----------- | ------------------------------ |
| Bloco protegido    | **try**     | Código que pode gerar erro.    |
| Captura erro       | **catch**   | Trata a exceção.               |
| Execução garantida | **finally** | Sempre executa.                |
| Lançar erro        | **throw**   | Lança uma exceção manualmente. |
| Declara exceção    | **throws**  | informa exceções possíveis.    |



____

7. Orientação a Objetos (escopo de herança).

| Uso                 | Palavras       | Observação                      |
| ------------------- | -------------- | ------------------------------- |
| Herança             | **extends**    | Classe herda outra.             |
| Implementação       | **implements** | Classe implementa interface.    |
| Referência pai      | **super**      | Acessa membros da superclasse.  |
| Referência atual    | **this **      | Refere-se ao próprio objeto.    |
| Verificação de tipo | **instanceof** | Testa se o objeto é de um tipo. |



____

8. Concorrência (escopo de threads).

| Uso                | Palavras         | Observação                          |
| ------------------ | ---------------- | ----------------------------------- |
| Execução paralela  | **synchronized** | Controle acesso concorrente.        |
| Thread cooperativa | **volatile**     | Garante visibilidade entre threads. |



____

9. Palavras reservadas não utilizada (legado).

| Uso            | Palavras            | Observação                          |
| -------------- | ------------------- | ----------------------------------- |
| Não utilizadas | **goto**, **const** | Reservadas, mas não usadas em Java. |



_____

