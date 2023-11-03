# 285_DesenvolvendoMicrosservicoJavaIntegracaoIAGenerativa



Desenvolvendo Microsserviço em Java para Integração com IA Generativa

- CONTEÚDOS
- INFORMAÇÕES

###### DESCRIÇÃO

Esse projeto tem como objetivo desenvolver um microsserviço responsável por receber uma imagem de perfil e enviá-la para uma Inteligência Artificial Generativa (Stable Diffusion), criando assim variações criativas da imagem. O microsserviço será desenvolvido em Java, utilizando o framework Quarkus e tecnologias avançadas como Hibernate, MariaDB, JAX-RS, Reactive Programming, Mutiny, Docker e Testcontainers. Você entenderá na prática desde criação da Estrutura do Projeto e seus Domínios até a conexão com Banco de Dados e o consumo de um serviço de IA via REST Client. Os pré-requisitos para conseguir executar o projeto por completo são: conhecimentos intermediários em Java e Docker, bem como conhecimentos básicos em HTTP, MariaDB e AWS S3.

**Java****Quarkus****Hibernate****Docker**

------

###### Full-Stack

###### Avançado

------

###### ESPECIALISTA

![author](https://hermes.dio.me/users/author/photos/8d12400e-5137-482a-bcac-ee0e3c47cdc6.jpg)

###### Thiago Poiani

Senior Java Developer, SkipTheDishes[**](https://www.linkedin.com/in/thpoiani/) [**](https://github.com/thpoiani/)

https://web.dio.me/lab/desenvolvendo-microsservico-em-java-para-integracao-com-ia-generativa/learning/633d291a-7924-4381-927c-8ac56220d063



[**](https://web.dio.me/play)

##### Desenvolvendo Microsserviço em Java para Integração com IA Generativa

**

[**](https://web.dio.me/lab/desenvolvendo-microsservico-em-java-para-integracao-com-ia-generativa/learning/633d291a-7924-4381-927c-8ac56220d063)[**](https://web.dio.me/lab/desenvolvendo-microsservico-em-java-para-integracao-com-ia-generativa/learning/b9d06e65-de76-4416-9c0a-47f55a602a7b)

<iframe id="ytc20" frameborder="0" allowfullscreen="1" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" title="Orientações Gerais - Visão Geral e Expectativas da Aula" width="100%" height="100%" src="https://www.youtube.com/embed/rqmlIsx8vQc?controls=0&amp;disablekb=1&amp;enablejsapi=1&amp;fs=0&amp;iv_load_policy=3&amp;modestbranding=1&amp;showinfo=0&amp;rel=0&amp;html5=1&amp;cc_load_policy=0&amp;origin=https%3A%2F%2Fweb.dio.me&amp;widgetid=1" data-gtm-yt-inspected-18="true" style="box-sizing: inherit; max-width: none; float: none; margin: 0px; padding: 0px; border: 0px; font-style: inherit; font-variant: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; font-family: inherit; font-optical-sizing: inherit; font-kerning: inherit; font-feature-settings: inherit; font-variation-settings: inherit; font-size: 14px; vertical-align: baseline;"></iframe>



03:37

 

09:18







normal

auto

- CONTEÚDOS
- INFORMAÇÕES

[Orientações Gerais - Visão Geral e Expectativas da Aula](https://web.dio.me/lab/desenvolvendo-microsservico-em-java-para-integracao-com-ia-generativa/learning/633d291a-7924-4381-927c-8ac56220d063)[Preparação do Ambiente e Configuração](https://web.dio.me/lab/desenvolvendo-microsservico-em-java-para-integracao-com-ia-generativa/learning/b9d06e65-de76-4416-9c0a-47f55a602a7b)[Estrutura do Projeto e Domínio](https://web.dio.me/lab/desenvolvendo-microsservico-em-java-para-integracao-com-ia-generativa/learning/597635bf-3953-4524-bdbb-0d5d017d860a)[Criação da API REST](https://web.dio.me/lab/desenvolvendo-microsservico-em-java-para-integracao-com-ia-generativa/learning/bb3df62b-ce9f-42cd-a53a-4111dbbbce11)[Conexão com o Banco de Dados](https://web.dio.me/lab/desenvolvendo-microsservico-em-java-para-integracao-com-ia-generativa/learning/6d7e05cf-1311-4815-9769-cae81fc0c3e3)[Armazenamento de Arquivos](https://web.dio.me/lab/desenvolvendo-microsservico-em-java-para-integracao-com-ia-generativa/learning/7fb0107f-07a2-4753-b1ca-738014992268)[Consumindo um Serviço de IA via REST Client](https://web.dio.me/lab/desenvolvendo-microsservico-em-java-para-integracao-com-ia-generativa/learning/2b9acbbe-e7e8-4bda-9cbe-5605b19954e3)[O Desafio Final](https://web.dio.me/lab/desenvolvendo-microsservico-em-java-para-integracao-com-ia-generativa/learning/acc17723-a96e-4a49-978b-0b093b9dc203)[Artigo de Referência](https://web.dio.me/lab/desenvolvendo-microsservico-em-java-para-integracao-com-ia-generativa/learning/2781c108-aebd-42c1-9ff5-9ad99eb324fb)[Entendendo o Desafio](https://web.dio.me/lab/desenvolvendo-microsservico-em-java-para-integracao-com-ia-generativa/learning/2ba664d7-1c87-486e-8570-5c1e5a814131)



# Entendendo o Desafio

**Agora é a sua hora de brilhar e construir um perfil de destaque na DIO! Explore todos os conceitos explorados até aqui e replique (ou melhore, porque não?) este projeto prático. Para isso, crie seu próprio repositório e aumente ainda mais seu portfólio de projetos no GitHub, o qual pode fazer toda diferença em suas entrevistas técnicas** 😎

*Dica: Se o expert forneceu um repositório Github, você pode dar um "fork" no repositório dele para organizar suas alterações e evoluções mantendo uma referência direta ao código-fonte original.*

### **Repositório Git**

O Git é um conceito essencial no mercado de trabalho atualmente, por isso sempre reforçamos sua importância em nossa metodologia educacional. Por isso, todo código-fonte desenvolvido durante este conteúdo foi versionado no seguinte endereço para que você possa consultá-lo a qualquer momento:
[**https://github.com/thpoiani/avatar**](https://github.com/thpoiani/avatar)

### **Slides**

Acesso aos slides utilizados pelo expert neste conteúdo:
**[Desenvolvendo Microsserviço em Java para Integração com IA Generativa.pptx](https://academiapme-my.sharepoint.com/:p:/g/personal/kawan_dio_me/EVD55oUvBIBKhualwDaalWkBBYoMlma76M2Sga6Qk-PMCA?e=cxJrXy)**

###  

Bons estudos 😉





