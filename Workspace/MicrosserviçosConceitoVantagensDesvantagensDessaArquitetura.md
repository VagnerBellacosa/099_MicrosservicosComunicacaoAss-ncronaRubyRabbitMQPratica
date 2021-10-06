# Microsserviços: conceito, vantagens e desvantagens dessa arquitetura

11 de Junho de 2020 

![img](https://secure.gravatar.com/avatar/bfe1116cfa4b587e6b3d5cecd337c70a?s=30)

 

## Entenda como funcionam os microsserviços e quais as vantagens e desvantagens deles

Sem tempo para ler este artigo? Aperte o play e escute!



Microsserviços. Eles nasceram em 2009, mas sua fama e popularidade começou realmente entre 2014 e 2015, quando o mercado reconheceu que o modelo de arquitetura era, de fato, atraente para o [**desenvolvimento de softwares em nuvem**](https://supero.com.br/solucoes/projetos/)**.** Desde então tem se consolidado como um **padrão cada vez mais comum e preferido pelos desenvolvedores**, sobretudo agora com o mundo se movendo para a cloud computing. 

O que é confirmado por dados. Pesquisa da [TechRepublic Premium](http://techrepublic.com/resource-library/whitepapers/research-microservices-bring-faster-application-delivery-and-greater-flexibility-to-enterprises/#link={"role":"standard","href":"https://www.techrepublic.com/resource-library/whitepapers/research-microservices-bring-faster-application-delivery-and-greater-flexibility-to-enterprises/","target":"","absolute":"","linkText":"Research: Microservices bring faster application delivery and greater flexibility to enterprise "}) realizada entre março e abril de 2020, com 447 profissionais, mostrou que os microsserviços estão no radar da maioria das empresas: 

- **96% afirmaram ter familiaridade com o conceito de microsserviços**. 
- **73% já integraram microsserviços** em suas aplicações. 
- Entre os que ainda não incorporaram a tecnologia, **63% pretendem** fazer isso. 

Em outra pesquisa, [esta da Kong](https://konghq.com/resources/digital-innovation-benchmark-2020/?utm_source=pressrelease&utm_medium=referral&utm_campaign=2020-innovation-report), 84% dos líderes de tecnologia consideram que os microsserviços estarão entre os motores da inovação e já o adotaram para acelerar os esforços de inovação e competitividade.

Para os entrevistados de ambas as pesquisas, no entanto, a **falta do conjunto de skills apropriadas**, bem como muitos [**sistemas legados**](https://supero.com.br/blog/sistema-legado-quando-esta-na-hora-de-reescrever/), e **falta de apoio corporativo** são as principais razões por que as organizações ainda não integraram microsserviços em suas aplicações ou têm dificuldade de escalar. 

Isso significa que, apesar de difundido o conceito de microsserviços, ainda há **pouca clareza sobre vantagens e desvantagens da tecnologia**. Então, é o que veremos neste post.

[![infográfico jornada para a cloud computing](https://supero.com.br/wp-content/uploads/2019/09/supero-pe%C3%A7as-supero-jornada-cloud-10-passos-cta-banner_v2.png)](https://materiais.supero.com.br/infografico-cloudcomputing)

### O que é microsserviços? 

É mais fácil explicar o que é arquitetura de microsserviços **contrastando-a com a arquitetura monolítica**, pois ela representa uma mudança do paradigma centralizador para um paradigma descentralizador de construção de aplicações. 

![monolito versus microsserviços](https://supero.com.br/wp-content/uploads/2020/06/monolito-versus-microsservi%C3%A7os-1-1024x469.png)

Segundo [Martin Fowler](https://martinfowler.com/articles/microservices.html): 

> Aplicativos monolíticos podem ser bem-sucedidos, porém serão frustrantes – especialmente quando mais [aplicações forem implementadas em nuvem](https://supero.com.br/blog/quando-migrar-para-a-cloud/). Ciclos de desenvolvimento são amarrados – uma mudança feita em uma pequena parte do aplicativo requer que o monolito inteiro seja republicado. Ao longo do tempo ficará cada vez mais difícil manter uma estrutura modular, o que torna mais difícil fazer com que mudanças afetem apenas um módulo. Escalar requer escalar o aplicativo inteiro, não apenas as partes que requerem mais recursos. 

Em contraste com a arquitetura monolítica, que funciona como um único serviço, a **arquitetura de microsserviços é a composição de um único software baseada em um conjunto de peças altamente especializadas, autônomas e simples**. 

Essa arquitetura tem um **acoplamento flexível e fraco** de suas partes. Isso significa que não é preciso considerar o impacto de cada componente no aplicativo como um todo: **cada um pode ser mantido por uma equipe pequena, escrito em uma linguagem própria, atualizado e modificado independentemente da aplicação principal e escalado à vontade**, sem recompilação e reimplantação do sistema como um todo. 

Até por serem cloud nativos, os microsserviços funcionam normalmente com [cloud computing](https://supero.com.br/solucoes/cloud/), ainda que não exclusivamente. 

### 6 vantagens dos microsserviços 

Em virtude das características elencadas acima, os microsserviços apresentam algumas vantagens imediatas para o desenvolvimento de softwares. Vejamos as principais: 

![vantagens dos microsserviços](https://supero.com.br/wp-content/uploads/2020/12/vantagens-dos-microsservi%C3%A7os.png)

#### 1. Facilidade e rapidez na atualização e implantação dos serviços 

Com microsserviços, atualizações e mudanças podem ser feitas **sem projetos e aprovações complexos**, pois são menores em escopo e independentes. 

Esqueça demorar semanas para fazer coisas relativamente simples. **A integração e a entrega são contínuas**. 

Por exemplo, se um serviço for atualizado, o aplicativo não precisa ser reimplantado; se algo der errado em uma atualização, ela é facilmente reversível. Isso sem falar nos bugs, que não interrompem o aplicativo ativo e nem comprometem lançamentos como um todo. 

A facilidade e a rapidez foram o **benefício mais citado** no levantamento da TechRepublic que citamos acima: para 69% dos entrevistados, essas são as maiores vantagens dos microsserviços. 

#### 2. Aumentar a flexibilidade da infraestrutura

Boa parte da rapidez e da facilidade vem da independência dos serviços entre si, ou seja, de sua flexibilidade. **Os componentes do aplicativo não precisam compartilhar código, modelos de dados e database comuns**. 

Minimizada a dependência entre os componentes, a **adição de funcionalidades e ferramentas melhores se dá de acordo com a necessidade**. 

Se os provedores de microsserviços mudarem completamente o hardware, a linguagem de programação ou a localização de seu data center, o usuário do serviço não será afetado. Assim, em aplicações de softwares internos, você não precisa se preocupar com o minucioso e caro trabalho de reescrever interfaces e conexões complexas entre sistemas se eles são entregues por microsserviços. 

Por isso, essa foi a segunda vantagem mais citada no levantamento da TechRepublic, lembrada por 61% dos entrevistados. 

#### 3. Escalabilidade 

Com microsserviços, cada serviço pode **escalar independentemente para atender uma demanda**. 

Isso significa que a **ampliação se torna bem dimensionada e precisa**, realizada apenas nos serviços que precisam dela, requerendo **menos infraestrutura** do que aplicativos monolíticos. 

Em virtude disso, esta vantagem foi citada por 56% dos entrevistados. 

#### 4. Estandardização de serviços 

Dentro da arquitetura de microsserviços, há vários **padrões de design, comunicação e de integração que ajudam a lidar com desafios** bem comuns, como backend-for-frontend (BFF), entidades e agregações, descoberta de serviços etc. 

Por isso, esse benefício foi citado por 42% dos entrevistados no levantamento de TechRepublic. 

#### 5. Redução de [**dívida técnica**](https://supero.com.br/blog/gerenciar-divida-tecnica/)

Como os componentes podem ser escalados e implementados independentemente dos outros, temos uma **redução considerável de custos e perdas associadas ao escalonamento dos aplicativos inteiro**, por exemplo. 

Tanto que esse benefício foi citado por 33% dos respondentes da pesquisa da TechRepublic. 

#### 6. Desenvolvimento de práticas DevOps e de colaboração do time

Segundo a [IBM](https://www.ibm.com/cloud/learn/microservices), a arquitetura de microsserviços reflete o modo como muitos líderes de negócios querem estruturar e conduzir seus times e processos de desenvolvimento. Nesse sentido, **o modelo arquitetôtico facilitaria um modelo operacional**. E ele tem a ver com [práticas DevOps](https://supero.com.br/blog/praticas-devops-para-implementar-agora/). 

Falamos acima que os serviços são mantidos por times pequenos. Disso, emerge, segundo a IBM, um modelo organizacional que reúne **times multidisciplinares em torno de um serviço ou conjunto pequeno de serviços**. 

Outra observação é que a **compreensão do código-base torna-se mais fácil por novos membros da equipe**, que os torna aptos a contribuir rapidamente. Desenvolvedores, portanto, não precisam mais compreender como os serviços funcionam a fundo para criar funcionalidades. 

### Por que a arquitetura de microsserviços pode ser útil a organizações? 

Para **grandes empresas**, adotar a arquitetura de microsserviços significa acabar com a dependência de um hardware particular ou de um software fornecedor. Ademais, elas podem ter sua infraestrutura melhorada sem afetar grande parte das aplicações. 

Já para **pequenos negócios e startups** pode ser uma forma de viabilizar projetos complexos. Se, antes, eles tinham uma quase intransponível desvantagem em relação às grandes empresas, que podiam bancar grandes data centers e uma grande equipe para mantê-los, a arquitetura de microsserviços democratiza mais esse acesso. 

Todas as organizações, potencialmente, podem acessar as APIs da Amazon ou do Google para usar seus ativos. Isso permite que softwares e aplicativos complexos sejam construídos rapidamente, usando serviços construídos e mantidos por outros. 

### Desvantagens da arquitetura de microsserviços 

Ora, depois de enfatizarmos tantos benefícios da arquitetura de microsserviços, será que ainda tem lugar para alguma desvantagem? Sim. 

E, se você está aqui porque cogita a migração para microsserviços, leia atentamente os pontos a seguir. 

**A maioria dos problemas que podem surgir com uso da arquitetura de microsserviços tem a ver, justamente, com sua lógica descentralizadora**, que apresenta – como tudo – prós e contras. 

#### 1. Complexidade 

É fácil perceber que **um sistema formado por partes autônomas e especializadas forma um todo bem complexo, distribuído**. Uma arquitetura monolítica, por outro lado, tem o benefício de ser um sistema centralizado e blocado. 

Por isso, seguindo Martin Fowler, especialista em arquitetura de software, “**não considere migrar para microsserviços a menos que você já tenha um sistema que seja muito complexo para gerenciar como um monolito**”. A IBM faz a mesma recomendação quando afirma: 

> Microsserviços são uma maneira de gerenciar complexidade quando softwares se tornaram muito grandes e incômodos para serem atualizados e mantidos facilmente. **Apenas considere como você pode fatorar o sistema em serviços menores quando você sentir a dor e complexidade de um monolito começando a afetá-lo**. Até que você não sinta essa dor, você não tem um monolito que precisa ser refatorado. 

Isso nos leva à consequência da complexidade: problemas com governança. 

#### 2. Governança 

Com vários componentes completamente distintos trabalhando juntos em um único aplicativo, a governança pode deixar a desejar. 

Segundo a Microsoft, “**estabelecer alguns padrões para todo o projeto, sem restringir excessivamente a flexibilidade das equipes**” é a solução que tem se mostrado mais útil. Investir em **deployment e automação do monitoramento** é a recomendação da IBM. 

Outro ponto é a cultura. Práticas DevOps maduras costumam ter mais sucesso. Veja que, se por um lado a adoção de microsserviços ajuda a consolidar práticas DevOps, por outro seu sucesso também depende de equipes que já tenham certa familiaridade com DevOps. 

#### 3. Integração com aplicações monolíticas legadas 

Como não se comunica com outros serviços, o uso da rede em um monolito é bem menor. Esse baixo tráfego de rede é uma vantagem que pode se perder na migração para microsserviços. 

Isso porque ter muitos pequenos serviços pode **gerar uma cadeia de comunicação extremamente prolixa e interdependente**, comprometendo o funcionamento da rede. 

#### 4. Segurança 

Algumas vulnerabilidades dos microsserviços são resultados diretos de sua natureza aberta, com uma ampla superfície sujeita a ataques. Sobretudo quando os microsserviços não estiverem bem definidos, documentados e estandardizados por meio de APIs seguras, a segurança também pode se tornar um problema.

##### Leia mais: [Como ter sucesso com microsserviços?](https://supero.com.br/blog/sucesso-com-microsservicos/)