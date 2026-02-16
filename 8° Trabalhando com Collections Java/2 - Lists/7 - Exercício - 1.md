```Java
package List;

  

import java.util.ArrayList;

import java.util.List;

import java.util.Collections;

  
  

public class Temperatura {

    public static void main(String[] args)

    {

        List<Mes> primeiroSemestre = new ArrayList<>()

        {{

  

            add(new Mes(1, "Janeiro", 28));

            add(new Mes(2, "Fevereiro", 27));

            add(new Mes(3, "Março", 26));

            add(new Mes(4, "Abril", 25));

            add(new Mes(5, "Maio", 24));

            add(new Mes(6, "Junho", 23));

  

        }};

        System.out.print(primeiroSemestre);

  

        double soma = 0;

  
  

        for(int i = 0; i < primeiroSemestre.size(); i++)

        {

            soma += primeiroSemestre.get(i).getTemperatura();

        }

  
  

        double media = soma / primeiroSemestre.size();

  
  
  

        for(int i = 0; i < primeiroSemestre.size(); i++)

        {

            if (primeiroSemestre.get(i).getTemperatura() > media)

            {

  

                System.out.println(

                    primeiroSemestre.get(i).getNome() +

                    " - " +

                    primeiroSemestre.get(i).getTemperatura()

                );

  

            }

        }

    }

}

  
  

class Mes {

  

    private Integer ordem;

    private String nome;

    private Integer temperatura;

  

    public Mes(Integer ordem, String nome, Integer temperatura){

  

        this.ordem = ordem;

        this.nome = nome;

        this.temperatura = temperatura;

  

    }

  

    public Integer getOrdem()

    {

  

        return ordem;

  

    }

  

    public String getNome()

    {

  

        return nome;

  

    }

  

    public Integer getTemperatura()

    {

  

        return temperatura;

  

    }

  

    @Override

    public String toString()

    {

  

        return "{" +

                " Ordem = " + ordem + '\'' +

                ", Nome = " + nome +

                ", Temperatura = " + temperatura + '\'' +

                '}';

  

    }

}
```