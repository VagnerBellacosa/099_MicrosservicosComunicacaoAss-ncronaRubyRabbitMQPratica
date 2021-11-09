# O que é Microserviços?

## **O que é microserviços?**

Microserviço é um tipo de arquitetura de software que organiza a aplicação em uma coleção de serviços fracamente acoplados.

Para compreender microsserviços, vamos antes conhecer algumas tipos de arquiteturas de software

### **Arquitetura Monolítica**

Muitos dos sistemas desenvolvidos são peças grandes e únicas de software, todo o código é desenvolvido em uma única linguagem de programação. É como se todo o software fosse um grande pacote. Esse tipo de arquitetura é muito comum e quase sempre mais simples de conceber. A este tipo damos o nome de “monólito”, ou dizemos que a arquitetura deste tipo de software é “monolítica”.

O problema deste tipo de aplicação é justamente sua estrutura monolítica. A menor alteração, mesmo que insignificante, exige o provisionamento da aplicação por completo. Algumas veze s adependencia é tão grande e amarrada que você altera uma parte e outra que não ‘tem nada a ver’, sofre as consequências.

A solução para este problema foi separar a aplicação em pedaços isolados menores. Com pedaços menores pode-se criar e espalhar réplicas das partes que mais exigiam das máquinas, dividindo a carga entre as réplicas, e também facilitando o provisionamento de novas versões, já que ao atualizar um pedaço isolado, o restante da aplicação não sofreria alterações.

### **Arquitetura Orientada a Serviços**

Uma abordagem para separar as aplicações monolíticas em serviços independentes apareceu antes dos anos 2000, e cresceu bastante em 2003 quando uma forma de comunicação entre processos chamada SOAP (Simple Object Access Protocol) ganhou sua versão 1.2 especificada pela W3C (World Wide Web Consortium). De lá para cá, o SOA (Service-Oriented Architecture) tem sido utilizado para o desenvolvimento de grandes arquiteturas, principalmente em aplicações que tratam de quantidades massivas de requisições. Nesta época as aplicações (ou serviços) conversavam diretamente entre si e não havia um padrão de comunicação, o que dificultava alterações e novas implementações. Mais ou menos nesses anos surge a figura do ESB (Enterprise Service Bus), uma espécie de tradutor comum para solucionar o problema entre todos os serviços.

Com o ESB as aplicações passaram a conversar de forma padrão, o ESB se encarregava de enviar as mensagens de um lado para o outro e conectava as diferentes partes.

Parece promissor, certo? Mas o ESB trouxe um problema, o próprio ESB, que passou a ser não somente um SPOF – Single Point of Failure – como também um possível gargalo entre as aplicações e suas mensagens. Existem diversas abordagens para evitar que isso aconteça, mas uma das abordagens, que acabou se tornando uma forma de implementação é justamente o que conhecemos como microsserviços.

### **Arquitetura de Microsserviços**

Após analisar tudo isso que foi dito acima, percebemos então que os microsserviços são então uma implementação específica do SOA em que os serviços conversam diretamente entre si – sem a figura do ESB – através de um protocolo e formato de dados padrão. Se você pensou em APIs REST está acompanhando o raciocínio!

Se os serviços podem se comunicar entre si, são mais tolerantes a falhas, pois podem haver várias réplicas de um mesmo serviço. Se a comunicação é um formato padrão, os serviços podem ser desenvolvidos em tecnologias diferentes. Cada pedaço pode ser provisionado individualmente, isoladamente, sem afetar a aplicação como um todo.

Os contêineres facilitaram drasticamente a adoção deste tipo de arquitetura.

## **O que é um container?**

Container é um pacote de uma aplicação que funciona de forma isolada do sistema operacional, com todas as suas dependências dentro de si. Uma aplicação autocontida que se comporta da mesma forma independente do ambiente em que está.

- Os containers são leves e contêm tudo o que é necessário para executar o aplicativo, portanto, você não precisa depender do que está instalado no host.

Se dentro de um container é possível colocar a aplicação e tudo o que ela precisa para poder rodar fica claro a dependência e a inter relação entre container e microsserviços.

## **Qual a diferença entre containers e Docker?**

Containers já existiam antes do Docker e incorporou a funcionalidade de containers a um serviço de fornecimento dos mesmos através da nuvem, tornando-os o alicerce de seu serviço.

O Docker oferece a capacidade de empacotar e executar um aplicativo em um ambiente isolado denominado container. O isolamento e a segurança permitem que você execute vários containers simultaneamente em um determinado host.

O Docker é uma plataforma aberta para desenvolvimento e execução de aplicativos. O Docker permite que os aplicativos sejam separados da infraestrutura para que possam entregar o software rapidamente. Com o Docker, você pode gerenciar sua infraestrutura da mesma forma que gerencia seus aplicativos e com isso reduzir significativamente o atraso entre escrever o código e executá-lo na produção.

## **Quais as vantagens de se usar microsserviços e containers?**

- Independência entre aplicativos e infraestrutura pois a infraestrutura ‘vem junto’ com o aplicativo;
- Ambiente completo para rodar aplicações minimizando os problemas das dependências;
- Menos recursos necessários, pois containers são mais leves que máquinas virtuais;
- Liberdade de escolha da linguagem de programação para os diferentes microsserviços;
- Os microsserviços podem mais facilmente serem reaproveitados em diferentes sistemas;
- Liberdade para escolha dos protocolos de comunicação entre os microsserviços.