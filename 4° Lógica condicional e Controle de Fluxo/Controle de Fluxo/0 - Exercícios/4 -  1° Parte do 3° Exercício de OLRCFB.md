


ifFlecha();

```Java 

/**

 * Classe de exemplo para o exercício da Aula 3 de Operadores lógicos e relacionais, Controle de Fluxo e Blocos.

 */
 
public class ExTres {

    public static void main(String[] args) {

        ifFlecha();

        ifSemFlecha();

        ifFerias();

        ifMenor();

  

        switchSemana();

        switchNumero();

        switchFerias();

  

    }

    private static void ifFlecha() {

  

        int mes = 2;

  

        if (mes == 1) {

            System.out.println("Janeiro");

        } else {

            if (mes == 2) {

                System.out.println("Fevereiro");

            } else {

                if (mes == 3) {

                    System.out.println("Março");

                } else {

                    if (mes == 4) {

                        System.out.println("Abril");

                    } else {

                        if (mes == 5) {

                            System.out.println("Maio");

                        } else {

                            if (mes == 6) {

                                System.out.println("Junho");

                            } else {

                                if (mes == 7) {

                                    System.out.println("Julho");

                                } else {

                                    if (mes == 8) {

                                        System.out.println("Agosto");

                                    } else {

                                        if (mes == 9) {

                                            System.out.println("Setembro");

                                        } else {

                                            if (mes == 10) {

                                                System.out.println("Outubro");

                                            } else {

                                                if (mes == 11) {

                                                    System.out.println("Novembro");

                                                } else {

                                                    if (mes == 12) {

                                                        System.out.println("Dezembro");

                                                    }

                                                }

                                            }

                                        }

                                    }

                                }

                            }

                        }

                    }

                }

            }

        }

    }


```

Efeito Flecha.

Esse efeito deve ser evitado ao máximo.

Quando se tem muitos if's, é sinal que o código está mal projetado.
Isso é uma má prática de programação.

O código não é feito para mim, e sim para outros desenvolvedores.


Inevitavelmente outras pessoas trabalharão sobre o meu código.

Por isso dessa forma que foi feito deve ser evitada.
___