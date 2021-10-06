# Microsserviços em poucas palavras

[Microservices](https://www.thoughtworks.com/microservices)[Blog](https://www.thoughtworks.com/pt-br/insights/blog) por [James Lewis](https://www.thoughtworks.com/en-br/profiles/j/james-lewis) e  [Martin Fowler](https://www.thoughtworks.com/pt-br/profiles/leaders/martin-fowler)

publicado: February 23, 2015 

*O termo "Arquitetura de Microsserviços (Microservice Architecture)" surgiu nos últimos anos para descrever uma maneira específica de desenvolver software como suites de serviços com deploy independente. Embora não exista uma definição precisa desse estilo de arquitetura, há certas características comuns em relação à organização, à capacidade de negócios, ao deploy automatizado, à inteligência nos terminais e ao controle descentralizado de linguagens e de dados.*

*O que segue foi retirado de um artigo que apareceu originalmente no* [website do Martin Fowler.](http://martinfowler.com/articles/microservices.html) 

"Microsserviços" - mais um novo termo nas ruas lotadas da arquitetura de software. Embora a nossa inclinação natural seja olhar para essas coisas com um certo desprezo, a terminologia descreve um estilo de sistemas de software que temos achado cada vez mais atraente. Temos visto muitos projetos usando esse estilo nos últimos anos, e os resultados até agora têm sido positivos; tanto que, para muitos de nossos colegas, microsserviços vem se tornando o estilo padrão para o desenvolvimento de aplicativos corporativos. Infelizmente, no entanto, não há muita informação que descreva o estilo de microsserviços e como aplicá-lo.

Resumindo, o estilo de arquitetura de microsserviços é uma abordagem que desenvolve um aplicativo único como uma suite de pequenos serviços, cada um executando seu próprio processo e se comunicando através de mecanismos leves, muitas vezes em uma API com recursos HTTP. Esses serviços são construídos em torno de capacidades de negócios e funcionam através de mecanismos de deploy independentes totalmente automatizados. Há o mínimo possível de gerenciamento centralizado desses serviços, que podem ser escritos em diferentes linguagens de programação e utilizam diferentes tecnologias de armazenamento de dados.

Para começar a explicar o estilo de microsserviços, é útil compará-lo com o estilo de aplicativo monolítico, construído como uma única unidade. Aplicativos corporativos geralmente são construídos em três partes principais: a interface de usuário do lado do cliente (que consiste em páginas HTML e JavaScript executadas em um navegador na máquina do usuário) um banco de dados (que consiste em muitas tabelas inseridas em um sistema de gerenciamento de banco de dados comum, geralmente relacional), e um aplicativo do lado do servidor. O aplicativo do lado do servidor lida com as solicitações HTTP, executa a lógica do domínio, recupera e atualiza dados do banco de dados, e seleciona e preenche as visualizações HTML a serem enviadas para o navegador. Esse aplicativo do lado do servidor é monolítico - um executável lógico único. Quaisquer mudanças no sistema envolvem criação e deploy de uma nova versão do aplicativo no lado do servidor.

O servidor monolítico é o caminho natural para abordar a construção de um sistema desse tipo. Toda a sua lógica para lidar com uma solicitação é executada em um único processo, o que lhe permite usar os recursos básicos de sua linguagem para dividir a aplicação em classes, funções e namespaces. Com um pouco de cuidado, você pode executar e testar o aplicativo no laptop de um desenvolvedor, usando um pipeline de deploy para garantir que as mudanças sejam devidamente testadas e colocadas em produção. Você pode escalar um aplicativo monolítico horizontalmente, executando muitas instâncias atrás de um balanceador de carga.

Aplicativos monolíticos podem funcionar bem, mas cada vez mais as pessoas estão se frustrando com eles, especialmente à medida que mais aplicativos vem tendo seus deploys na nuvem. Ciclos de alterações são vinculados - uma alteração feita uma pequena parte do monolito requer que todo ele seja reconstruído e que o deploy seja refeito. Ao longo do tempo muitas vezes é difícil manter uma boa estrutura modular, o que dificulta mantermos as alterações que devem afetar apenas um módulo de dentro do módulo. Escalar requer o redimensionamento de todo o aplicativo, ao invés de partes que exigem mais recursos.

![img](https://www.thoughtworks.com/content/dam/thoughtworks/images/photography/inline-image/insights/blog/microservices/blg_inline_microservices_nutshell.jpg)

Essas frustrações levaram à criação do estilo de arquitetura de microsserviços: construir aplicativos como suites de serviços. Assim como os serviços têm deploy independente e são escaláveis, cada serviço também possui um limite de módulo firme, que permite inclusive que diferentes serviços sejam escritos em diferentes linguagens de programação. Eles também podem ser gerenciados por equipes diferentes.

Não estamos afirmando que o estilo de microsserviços seja novo ou inovador, suas raízes remontam, pelo menos, aos princípios de design do Unix. Mas realmente pensamos que ainda são poucas as pessoas que consideram uma arquitetura de microsserviços e que muitos desenvolvedores de software se beneficiariam dessas informações.

**Saiba mais:**

O artigo de James e Martin prosegue com a definição de o que é uma arquitetura de microsserviços expondo 9 características comuns, discutindo sua relação com a Arquitetura Orientada a Serviços, e refletindo sobre se este estilo é o futuro do software corporativo. Leia aqui: [martinfowler.com/articles/microservices.html](http://martinfowler.com/articles/microservices.html). 

