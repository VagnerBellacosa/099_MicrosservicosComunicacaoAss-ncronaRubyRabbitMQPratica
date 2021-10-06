[![imagem destaque](https://www.opus-software.com.br/wp-content/uploads/2021/03/pexels-pixabay-373543-1210x423.jpg)](https://www.opus-software.com.br/wp-content/uploads/2021/03/pexels-pixabay-373543-1030x687.jpg)

# [Micro Serviços: Qual a diferença para a Arquitetura Monolítica?](https://www.opus-software.com.br/micro-servicos-arquietura-monolitica/)

17/03/2021/por [OPUS Software](https://www.opus-software.com.br/author/wpuser/)

O termo **micro serviços** foi criado em maio de 2011 durante uma conferência de arquitetos de software para representar um **estilo de arquitetura de sistemas** e, não exatamente, o tamanho dos serviços que a compõe, como o nome pode sugerir. 

A proposta da arquitetura orientada a micro serviços é desenvolver sistemas que sejam mais **flexíveis**, **escaláveis** e com **manutenção** mais **simples** do que as arquiteturas de sistemas monolíticos, que normalmente são utilizadas. 

Portanto, a principal filosofia desta arquitetura é “**fazer uma coisa e fazê-la bem**”, por isso os serviços são focados em realizar uma única função. 

Essa filosofia não é uma novidade na área de sistemas. McIlroy, Pinsen e Tague, pioneiros do sistema UNIX, já haviam publicado sobre esse conceito em 1978 no clássico artigo “[Unix Time-Sharing System: Forward](https://archive.org/details/bstj57-6-1899)”. Revisitar esse conceito e aplicá-lo ao contexto das tecnologias atuais certamente pode trazer muitos benefícios para os times de tecnologia. 

Pensando nisso, nesse post nós vamos apresentar como funciona cada uma das arquiteturas, a monolítica e a de micro serviços, assim como os impactos positivos que essa última pode trazer para a empresa e como o open banking e os micro serviços podem estreitar relações. 

- - [Como funciona a arquitetura monolítica ](https://www.opus-software.com.br/micro-servicos-arquietura-monolitica/#a)
  - [Como funciona a arquitetura de micro serviços ](https://www.opus-software.com.br/micro-servicos-arquietura-monolitica/#b)
  - [Por que os micro serviços são importantes para os negócios? ](https://www.opus-software.com.br/micro-servicos-arquietura-monolitica/#c)
  - [Fatores relevantes para adotar a arquitetura de micro serviços ](https://www.opus-software.com.br/micro-servicos-arquietura-monolitica/#d)
  - [Micro serviços e Open Banking ](https://www.opus-software.com.br/micro-servicos-arquietura-monolitica/#e)

## **Como funciona a arquitetura monolítica** 

As principais linguagens de desenvolvimento de aplicações oferecem abstrações para quebrar a complexidade dos sistemas em módulos. Entretanto, são projetadas para a criação de um único executável **monolítico**, no qual **toda a modularização utilizada é executada em uma mesma máquina**. Assim, **o****s módulos compartilham recursos de processamento, memória, bancos de dados e arquivos**. 

Uma arquitetura monolítica típica de um sistema complexo pode ser representada pela figura abaixo, na qual todas as funções do negócio estão implementadas em um único processo. 

![micro-servicos-arquitetura-monolitica](http://www.opus-software.com.br/wp-content/uploads/2017/02/micro-servicos-arquitetura-monolitica.png)

### **Desafios da arquitetura monolítica**  

Ao longo do tempo o sistema vai crescendo, se tornando mais complexo e consumindo cada vez mais recursos, o que acaba gerando também alguns desafios substanciais para a manutenção desse tipo de arquitetura. São eles: 

#### **Aumento d****a** **complexidade e tamanho ao longo do tempo** 

O sistema se torna tão complexo que a manutenção fica cada vez mais cara e lenta, porque os desenvolvedores têm que navegar em uma infinidade de códigos. 

#### **Alta dependência de componentes de código**

Muitas funções são interdependentes e entrelaçadas, de forma que a inclusão ou manutenção de componentes do sistema pode causar inconsistências ou comportamentos inesperados. 

#### **Escalabilidade do sistema é limitada** 

Mesmo que apenas parte da funcionalidade seja necessária na nova instância, uma arquitetura monolítica exige que todo o sistema seja replicado, o que gera custos maiores do que o esperado. 

#### **Falta de flexibilidade** 

Exige que os desenvolvedores fiquem amarrados à tecnologia originalmente escolhida para o sistema, mesmo que em algumas situações ela não seja a melhor escolha. 

#### **Dificuldade para colocar alterações em produção** 

Qualquer mudança, por menor que seja, requer a reinicialização do sistema. Como isso pode causar algum risco operacional, é necessário que as equipes de desenvolvimento, testes e manutenção desses sistema acompanhem essas alterações. 

## **Como funciona a arquitetura de micro serviços** 

A arquitetura de micro serviços é utilizada para desenvolver uma aplicação como um **conjunto de pequenos serviços**, que funcionam com seu próprio processo. Cada serviço é desenvolvido em torno de um conjunto de **regras** de negócio **específic****as**, e é implementado de forma **independente**. 

Com isso, é possível quebrar algumas barreiras existentes no modelo de arquitetura monolítica. 

### **Benefícios dos micro serviços** 

#### **Manutenção e evolução dos serviços mais estáveis** 

Como os desenvolvedores vão trabalhar com códigos que executam uma única função, os serviços individuais não vão acompanhar o potencial crescimento do sistema, evitando que você precise carregar uma parte desnecessária da aplicação. 

#### **Serviços com baixo nível de acoplamento e interdependência** 

A manutenção em um serviço específico não interfere diretamente nas outras funcionalidades do sistema. 

#### **Escalabilidade do sistema**

Os deploys e replicações de micro serviços são feitos por meio de infraestruturas de servidores, máquinas virtuais e containers que se organizam de forma independente. Isso torna o crescimento e a possibilidade de adaptação do sistema muito mais flexível. 

#### **Redução de custos** 

Cada aplicação só utiliza os serviços que necessita. Por isso, você não vai ter gastos extras carregando funcionalidades não utilizadas, afinal os custos estão diretamente associados à funcionalidade e à carga de uso do sistema. 

#### **Flexibilidade de tecnologia** 

Por conta do baixo acoplamento entre os serviços, não é necessário amarrar os desenvolvedores a uma tecnologia específica, o que te permite escolher a melhor opção para atender cada caso. 

Isso diminui os riscos de obsolescência tecnológica e possibilita a evolução constante do sistema. 

#### **Facilidade de colocar alterações em produção** 

As mudanças no sistema são executadas por meio de alterações e evoluções feitas nos serviços. Portanto, o sistema como um todo não precisa ser reinicializado para continuar funcionando. 

Assim, o time de desenvolvimento que vai precisar acompanhar a mudança será apenas o de responsáveis pelos serviços que estão sendo alterados. 

## **Por que os micro serviços são importantes para os negócios?** 

Naturalmente, faz parte dos objetivos das empresas acompanhar os avanços do mercado para evoluir constantemente, conquistar cada vez mais excelência, aumentar a agilidade na criação de novos produtos e serviços, criar diferenciais competitivos e, claro, reduzir custos. 

Para que esses objetivos possam ser alcançados, a arquitetura das aplicações também precisa evoluir. Mas o que não pode faltar nessas aplicações? 

- **Foco** **na experiência do usuário:** dinamismo e interatividade são conceitos que não podem ficar de fora quando o assunto é entregar valor para o usuário, independentemente da plataforma (o que inclui também os dispositivos móveis); 
- **Escalabilidade:** as aplicações desenvolvidas precisam estar altamente disponíveis. Além disso, deve ser possível executá-las em ambientes de nuvem; 

- **Atualizações** **suaves****:** o ideal é que as atualizações não ocasionem paradas ou instabilidades que prejudiquem os usuários. 

A arquitetura orientada a micro serviços viabiliza a construção de sistemas que possuem todos essas características que citamos acima, diferentemente das aplicações monolíticas. 

Os micros serviços permitem: 

- Que novos processos ou serviços sejam disponibilizados sem impactar os processos e serviços existentes; 
- Alterações em processos e serviços sem a necessidade de parada de todo o sistema; 
- Otimização da utilização da infraestrutura de nuvem; 
- Redução da complexidade de manutenção. 

Dessa maneira, a implementação de novos serviços pelo time de desenvolvimento ao longo do ciclo de vida da aplicação se torna muito mais simples e rápida. 

## **Fatores relevantes para adotar a arquitetura de micro serviços** 

Na análise de Martin Fowler, autor reconhecido na área de arquitetura de software, um sistema complexo que utiliza micro serviços tem um custo de manutenção menor do que o de aplicações com arquitetura monolítica, como exemplificado no gráfico a seguir: 

[![micro-servicos-Martin-Fowler](http://www.opus-software.com.br/wp-content/uploads/2017/02/micro-servicos-Martin-Fowler.png)](https://martinfowler.com/bliki/MicroservicePremium.html)

Ganho de produtividade vs. Aumento de complexidade do sistema Martin Fowler – Microservice Premium

 

Entretanto, existe uma barreira que pode impactar a adoção de uma arquitetura baseada em micro serviços: o custo na entrada, quando comparamos esse valor com o de um sistema monolítico. Além disso, eventualmente, pode existir a necessidade de um esforço extra para a gestão dos micros serviços que deve ser considerado também. 

Os grandes players do mercado podem ver isso como uma oportunidade para fornecer ferramentas que auxiliem os times na gestão dos micros serviços, com o objetivo de diminuir a barreira de entrada para a adoção dessa arquitetura, tendo em vista os benefícios a médio e longo prazo que ela oferece. 

Por exemplo, a Microsoft já atua nesse sentido com o [Azure Service Fabric](https://azure.microsoft.com/pt-br/services/service-fabric/). Esse recurso pretende atuar como middleware para facilitar a criação e gerenciamento de micro serviços em nível corporativo. Além disso, uma característica interessante do Service Fabric é que ele funciona independentemente da plataforma estar ou não na nuvem. 

Não podemos deixar de mencionar também os possíveis riscos da adoção da arquitetura de micro serviços traz. Afinal, como estamos falando de sistemas complexos sempre há pontos que demandam mais atenção, independente da arquitetura escolhida. 

No caso dos micro serviços, é necessário prestar atenção no(a): 

- Aumento da complexidade da coordenação; 
- Comunicação entre os micro serviços; 
- Governança. 

Portanto, para obter sucesso na adoção da arquitetura de micro serviços, esses fatores devem ser bem planejados e adequados para que a execução possa fazer parte da agenda da área de tecnologia da organização. 

## **Micr****o** **serviços e Open Banking** 

Agora que você já conhece as principais características da arquitetura de micro serviços, vamos apresentar um caso em que essa estrutura pode ser aplicada: no desenvolvimento da [api open banking](https://www.opus-software.com.br/api-open-banking/). 

O [open banking](https://www.opus-software.com.br/open-banking-o-que-e/) é uma iniciativa global que tem como objetivo permitir que os clientes possam compartilhar seus dados financeiros com outras instituições, por meio de APIs. 

Pensando nisso, ao desenvolver a api open banking, você poderá optar pela arquitetura de microsserviços. Isso porque, os bancos e instituições financeiras – que são os principais atores das próximas fases do open banking no Brasil – oferecem uma série de serviços, que podem estar estruturados para operar de forma independente no sistema, facilitando a atualização, manutenção ou a mobilidade, evitando atrasos, lentidão e alteração no tempo de resposta. 

O [gerenciamento de APIs](https://www.opus-software.com.br/importancia-do-gerenciamento-de-apis/) eficaz é peça fundamental no desenvolvimento do open banking, permitindo a integração de serviços financeiros às diferentes jornadas digitais dos clientes e reduzindo a diferença de informações entre os prestadores de serviços, favorecendo o surgimento de novos modelos de negócios e de novas formas de relacionamento entre instituições e seus clientes e parceiros. 

\>>Leitura recomendada: [Open banking Brasil: descubra os principais desafios e impactos da implementação no mercado financeiro](https://www.opus-software.com.br/open-banking-brasil/)