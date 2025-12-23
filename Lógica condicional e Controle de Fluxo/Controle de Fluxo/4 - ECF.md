Sobre os exercícios de Controle de Fluxo

____

Em Alguns casos o comportamento padrão do switch, assumiu um valor de negócio.

Pegou o comportamento padrão e transformou ele em um comportamento esperado, o que é errado. 

O comportamento padrão deve ser usado para notificarmos sobre algo de errado/inesperado.

Como falamos sobre o switch, nele utilizamos o default.

Ou seja, como forma de boas práticas nunca se deve utilizar o default de um switch, para ter um comportamento padrão.
Ele deve ser utilizado para identificarmos situações inesperadas, caso haja algo de errado no nosso código, por valor que estamos querendo testar.

___