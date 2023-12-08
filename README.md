![image](https://github.com/AndreCoutinhom/alura_software_engineering_education/assets/91290799/12360cca-f0ea-4834-b992-62eb733d295b)

# Engenharia de Software

Engenharia de software é uma das áreas da computação cujo foco está relacionado com análise, desenvolvimento e manutenção de softwares, bem como gestão de projetos e times.

É uma área bastante extensa, pois contempla as diversas disciplinas necessárias durante todo o processo de criação e manutenação de softwares, tais como:

* Gestão de requisitos;
* Arquitetura e design de sistemas;
* Padrões de projeto;
* Banco de dados;
* Testes de software;
* Gestão de projetos;
* Infraestrutura e deploy.

A formação engenharia de software da Alura está organizada com diversos conteúdos que contemplam tais disciplinas, de maneira que você possa adquirir os conhecimentos necessários para ter uma boa visão sobre esta área tão importante da computação.

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

# Clean Architecture

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

