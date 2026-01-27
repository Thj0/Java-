
# Terminal e Argumentos 

Nem sempre executamos nosso programa Java pela IDE, já pensou nossos clientes tendo que instalar o Eclipse ou VsCode para rodar o sistema em sua empresa?

Com a JVM devidamente configurada, nós podemos criar um executável do nosso programa e disponibilizar o instalador para qualquer sistema operacional. 

No nosso caso iremos aprender como executar um programa Java via terminal como MS - DOS ou terminal do VsCode.

Vamos criar uma classe chamada MinhaClasse.java com o código abaixo: 

```
public class MinhaClasse { 
	public static voi main(String[] args) {
		System.out.println("Fui executado pelo terminal");
	}
}
```

No nosso projeto Java criado pela IDE, teremos uma pasta chamada **bin**. É nessa pasta que fica m os arquivos **.class**, o nosso bytecode.

Mesmo usando uma IDE, nós sempre precisaremos identificar aonde se encontram as classes do nosso projeto.

Ex: C:\Decoding\DIO-Basic-Java-

___
# Terminal 

Agora será mostrado como executar uma classe, depois de compilada, sem precisar usar a IDE.

1. Abra o MS-DOS ou Power Shell.
2. Localiza o diretório do seu projeto: **cd C:\Decoding\DIO-Basic-Java-Java Terminal**
3. Acesse a pasta bin: **cd bin/**
4. Agora digitemos o comando : **java MinhaClasse** (o nome da sua classe sem a extensão .java).

___

