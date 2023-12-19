# Design e Arquitetura

## Design de Código vs Arquitetura de Software

A principal diferença entre design de código e arquitetura de software está em seus diferentes níveis de padrão.

Enquanto Design de Código é focado no posicionamento e sintaxe do código em si, a Arquitetura de Software se trata do conhecimento de alto padrão sobre a organização e funcionamento esquemático de todos os componentes do software.

## Arquitetura Hexagonal

### O que deve ser feito?:

* Definier quais componentes criar.
* Como os componentes serão organizados na aplicação.

### Padrão Ports and Adapters

![image](https://github.com/AndreCoutinhom/alura_software_engineering_education/assets/91290799/7c1b93f8-e4fd-40c5-b481-e3493d8ef97a)


### O que significa?

A ideia é construir sistemas que favorecem reusabilidade de código, alta coesão, baixo acoplamento, independência de tecnologia e que são mais fáceis de serem testados.

* Primary Adapters são receptores de dados.
* Secondary Adapters são displays desses dados.


### [DDD (Domain-Driven-Design)](https://www.amazon.com.br/Domain-driven-design-atacando-complexidades-software/dp/8550800651?source=ps-sl-shoppingads-lpcontext&ref_=fplfs&psc=1&smid=A1ZZFT5FULY4LN)

Foco na modelagem de software para corresponder a um domínio de acordo com as informações dos especialistas desse domínio.

## Clean Architecture

### MVC (Model View Controller)

![image](https://github.com/AndreCoutinhom/alura_software_engineering_education/assets/91290799/845284d2-2eb4-4d9a-af4b-6b207a774582)

* O MVC é uma forma de organizar a aplicação web, mas ainda é necessário definir cada campo.

### Clean Architecture 

![image](https://github.com/AndreCoutinhom/alura_software_engineering_education/assets/91290799/1aef2c26-3444-4ebe-ae65-1f666eb819be)

* Uma entidade é um tipo de classe que possui alguma identidade. Onde ficam as regras do negócio.
* Use cases são classes que organizam o fluxo das regras de negócio.
* A camada de adaptadores transfere dados externos para o sistema.
* A última camada é totalmente ligada à infraestrutura do negócio que interage com o usuário.

> O ideal de uma arquitetura limpa é manter algumas camadas não dependentes da infraestrutura. Por exemplo, a última camada pode envolver mudanças na linguagem de programação ou na estrutura do banco de dados, mas as regras do negócio permaneceriam as mesmas.

## Domain-Driven Design

### Padrões estratégicos

* Linguagem Ubíqua (onipresente)
* Contextos delimitados
* Domínio e Subdomínio (o que define o núcleo do funcionamento da empresa?)

### Padrões táticos

* Entidades
* Repositórios
* Eventos
* Módulos
* Serviços

> DDD está mais para uma filosofia de produção

![image](https://github.com/AndreCoutinhom/alura_software_engineering_education/assets/91290799/3436e8c8-8940-46c4-8830-004249d17ba2)

## Mensageria

![image](https://github.com/AndreCoutinhom/alura_software_engineering_education/assets/91290799/e3cbc8fa-b517-433d-a1e9-b5aabbd41aff)


* É uma conduta de envio de mensagens assíncronas.
* Nessa conduta é possível que mensagens de aviso sejam enviadas sem que o processo de construção seja interrompido.

> Exemplo em código:

![image](https://github.com/AndreCoutinhom/alura_software_engineering_education/assets/91290799/5f818b02-2ab2-4552-bf87-e2794534a523)

## Modelagem de eventos

* Consolidado por Adam Dymitruk

### Fases

* Brainstorming;
* Ordenação lógica (the plot);

![image](https://github.com/AndreCoutinhom/alura_software_engineering_education/assets/91290799/62c7fdfe-3f19-42f7-a6e8-0413c8c6eb0b)

* Storyboard;
* Identificando entradas;
* Identificando saídas;
* Lei de conway;
> Separação lógica dos eventos referente à estrutura empresarial (quem faz o quê)
* Elaboração de cenários.

## Arquitetura orientada a eventos

### Escabilidades

Formas de adequar o serviço diante de aumento de complexidade

* Horizontal;
> Busca soluções adicionando o número de serviços e tecnologias para a aplicação.
* Vertical;
> Busca soluções envolvendo o aumento quantitativo de recursos de produção (hardware)
* Profundidade
> Busca soluções em forma de mudanças relacionadas ao cenário e ao público foco. Geralmente aplicado como inovação.

### Event Bus

* Sistema baseado em comunicação de eventos por mensageria.

![image](https://github.com/AndreCoutinhom/alura_software_engineering_education/assets/91290799/7a22b918-d2cb-41cb-b581-11dc55df5b93)

### Event sourcing

* Sistema baseado em implementações de evento (controle de versão)




