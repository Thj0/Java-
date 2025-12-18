# Organizando Arquivos 

À medida que nosso sistema vai evoluindo, surgem novos arquivos (código fonte) em nossa estrutura de arquivos do projeto. Isso exige que seja realizado uma organização destes arquivos através de pacotes (packages).



____

As empresas costumam utilizar como base o próprio **domínio do site**, e não o segmento da empresa. O domínio, quando invertido, determina o prefixo principal do package.

Alguns exemplos comuns de domínios:



1. **.com** – Empresas comerciais
2. **.org** – Organizações e fundações sem fins lucrativos
3. **.io / .dev / .net / .edu** – Usados por projetos modernos, empresas de tecnologia, redes, universidades, etc.



**Esses prefixos vêm do domínio do site**, *não do tipo de arquivo ou projeto*.

Por isso se utiliza o **domínio invertido** como base do package.

E assim sucessivamente.



____

Dentro dos nossos projetos, existem finalidades.

Grande parte dos projetos possuem essas propostas no que se diz:



- **com** – geralmente aparece porque o domínio da empresa é .com
- **org** – geralmente aparece porque o domínio da organização é .org
- **io / dev / net / etc.** – aparecem conforme o domínio utilizado pelo projeto



:heavy_exclamation_mark:

> **Não existe o prefixo “opensource” como domínio.
>  Projetos opensource normalmente usam `.org` porque suas fundações registram domínios .org, e não porque o projeto “é opensource”.**



Esses prefixos são aplicados na maioria dos projetos.

Porém, não são usados porque a empresa é comercial, organizacional ou opensource, mas porque:

____

### Usam o “domínio invertido” para garantir unicidade dos pacotes

Isso evita conflito entre pacotes como:

`com.google.something`
 `com.microsoft.something`
 `org.apache.commons`

Cada empresa tem um domínio único → pacotes únicos.



Então, algumas vezes os projetos iniciarão com;

org, com, io, dev, etc.

(depende do domínio oficial registrado pela empresa ou pelo projeto)



____

Exemplo: 

// Nome da empresa

Tryvon



Domínio: tryvon.com

package raíz: 



com.tryvon.notification



Após isso;

____

Dentro desse pacote eu posso ter subfinalidades.

Posso ter pacotes chamados de:



com.tryvon.notification.app - "app" Para inicializar aplicação 

com.tryvon.notification.model - "model" Para colocar as classes de modelo 

com.tryvon.notification.util - "util" De utilidades

com.tryvon.notification.service - "service" Um pacote onde contém todas as regras de serviços/ regras de negócios.

____



