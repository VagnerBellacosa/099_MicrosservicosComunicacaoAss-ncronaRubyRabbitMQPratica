# [RabbitMQ] Introdução ao mundo das filas

### #### [MARCELA SISILIANI DE SENA SILVA](https://imasters.com.br/perfil/marcelasisilianisena)

Backend Developer multi stack no Grupo Bandeirantes, mas como uma boa cientista da computação curte mesmo é investigar (alá Sherlock) e conhecer novas tecnologias (surfando na onda Go). Gateira e crê que dividir é multiplicar!

[LEIA MAIS](https://imasters.com.br/perfil/marcelasisilianisena) 10 ABR, 2019

### [Azure – Como criar uma base de dados SQL no Microsoft Azure pronta para ser utilizada](https://imasters.com.br/banco-de-dados/azure-como-criar-uma-base-de-dados-sql-no-microsoft-azure-pronta-para-ser-utilizada)

18 MAR, 2019

### [Golang: como ler um arquivo json](https://imasters.com.br/back-end/golang-como-ler-um-arquivo-json)

Fala, pessoal!

O que as filas têm em comum com a programação? Como podemos resolver problemas do cotidiano usando filas? E o que é o RabbitMQ?

Bem-vindos a mais um artigo! Hoje vamos falar de **filas**! Isso mesmo, um assunto polêmico, mas necessário para contornar problemas e aperfeiçoar nossas soluções.

## O que são filas?

Que as filas fazem parte do nosso dia a dia não é novidade pra ninguém, certo? Podemos não associar à matemática, estatística e probabilidade, mas as encontramos no banco, no restaurante, no cinema (mesmo com lugar marcado). Já vi até uma fila de uma fila.

A definição de fila na [Wikipédia](https://pt.wikipedia.org/wiki/Teoria_das_filas) diz:

- **A teoria das filas é um ramo da [probabilidade](https://pt.wikipedia.org/wiki/Probabilidade) que estuda a formação de [filas](https://pt.wikipedia.org/wiki/FIFO), através de análises [matemáticas](https://pt.wikipedia.org/wiki/Matemática) precisas e propriedades mensuráveis das filas. Ela provê modelos para demonstrar previamente o comportamento de um sistema que oferece serviços cuja demanda cresce [aleatoriamente](https://pt.wikipedia.org/wiki/Aleatoriedade), tornando possível dimensioná-lo de forma a satisfazer os clientes e ser viável economicamente para o provedor do serviço, evitando desperdícios e gargalos.**

Então, com a ajuda da matemática, mais precisamente da probabilidade junto à tecnologia, podemos dimensionar as filas que encontramos por aí, dividi-las em processos e tornar o mundo muito mais fluído.

## Exemplos de uso de filas na programação?

Sendo assim, na área de programação o conceito de filas pode ser (e são) aplicados em várias soluções do cotidiano. Há filas em resoluções das corriqueiras, como na busca de motorista da Uber ou na indicação de filmes da Netflix, até as mais complexas, como softwares de análise combinatórias genéticas usadas para fila de transplante de órgãos.

E é por conta desse conceito matemático que somos capazes de desenvolver aplicações elegantes para problemas como:

- Análise de falhas em determinado processo. Exemplo: o por quê de um fluxo demorar mais para ser executado em determinada parte do dia ou se é necessário aumentar a quantidade de atendentes de um serviço de atendimento ao cliente
- Crescimento inesperado do fluxo de dados
- Gargalo na infraestrutura do projeto
- Alteração e inserção de grande massa de dados na base
- Processamento de quantidades gigantescas de informações

Esses e muitos problemas podem ser solucionados em background, ou seja, por baixo dos panos, sem que nosso usuário final seja impactado negativamente pela demora de salvar um documento, processar a compra em um e-commerce ou até mesmo esperar um carro do Uber na chuva até ficar encharcado.

O ramo matemático que estuda filas é bem extenso, e apesar de muita gente achar que não é diretamente ligado a programação, **recomendo** que estudem esse tema a fundo! Com toda certeza se tornarão programadores **muito** melhores!

## O que é RabbitMQ?

Para explicar o que é [RabbitMQ](https://www.rabbitmq.com/tutorials/tutorial-one-go.html), vou usar a analogia do site oficial (tradução livre), que diz:

- **Você pode pensar que somos como um serviço postal. Quando você coloca uma carta na caixa de correio, você tem certeza que o remetente vai recebê-la. Nessa analogia, o RabbitMQ é a caixa de correio, o serviço de entregas e o carteiro. A diferença entre o RabbitMQ e um serviço de entregas é que no lugar de papel, armazenamos e entregamos blocos binários de dados: as mensagens.**

Continuando a analogia, depois que você envia uma carta pra alguém, você não fica na frente da agência postal esperando até a pessoa receber a mensagem (já pensou esperar a resposta de um amigo que tá na lá Austrália? Que loucura, né?).

Você vai viver sua vida enquanto tem alguém (os Correios, por exemplo) trabalhando pra entregar a carta, certo? Pois bem, o RabbitMQ é o mensageiro da sua aplicação.

Importante salientar as seguintes características do RabbitMQ:

- É open-source (três vivas para softwares livres e de qualidade)
- Utiliza o AMQP (Advanced Message Queuing Protocol), que é um protocolo de comunicação em rede para rotear e distribuir as mensagens de aplicações
- Tem suporte em várias clouds, e nas principais aqui no Brasil, como GCP, AWS e Microsoft Azure, entre tantas outras
- Conteúdo vasto no [site oficial](https://www.rabbitmq.com/) (em inglês)

É novo no RabbitMQ? Tem [tutoriais no estilo ‘Hello Work’](https://www.rabbitmq.com/getstarted.html) (em inglês) em várias linguagens de programação, além do nosso queridinho Go.

## Composição básica das filas

Apesar de existirem diversos padrões de filas, você poder escolher qual é o melhor para sua solução. Em todos os tipos de cenários possuímos ao menos os três elementos a seguir: **Producing**, **Queue**, **Consuming**.

## Producing – O produtor da mensagem

Como diz o nome, é a aplicação que produz a mensagem e a insere na fila.

![img](https://static.imasters.com.br/wp-content/uploads/2019/05/27144455/0_-p64meEqGDPMSlz0.png)

## Queue – A fila

É a caixa postal – a fila – que fica dentro do RabbitMQ e aloca as mensagens enviadas pela sua aplicação. A única limitação para uma fila é a memória de um servidor ou o limite do seu disco. Uma fila pode ser abastecida e consumida por mais de uma aplicação.

![img](https://static.imasters.com.br/wp-content/uploads/2019/05/27144530/0_S3BlrWTqsKWrD1aI.png)Representação de uma fila na documentação do RabbitMQ

## Consuming – O recepetor da mensagem

Esse é o destinatário da nossa mensagem. Geralmente é uma aplicação em que a principal função é receber e processar a mensagem alocada na fila.

![img](https://static.imasters.com.br/wp-content/uploads/2019/05/27152537/0_UgBYosvhFXGcGUZK.png)

Geralmente, cada um desses elementos estão em um servidor diferente.

![img](https://static.imasters.com.br/wp-content/uploads/2019/05/27152741/1_Hf4e8ZffdzeAng5q4dntyw.png)Exemplificação básica de uma fila

## Os cinco padrões de implementação de filas no RabbitMQ

Como um bom mensageiro, o nosso coelho (mascote do RabbitMQ) tem diversas formas para implementar sua utilização de acordo com a necessidade da solução.

São elas: **Work Queues**, **Publish/Subscribe**, **Routing**, **Topics**, **RPC**.

Abaixo falo de cada uma resumidamente:

### Work queues – Distribuindo tarefas entre serviços

Utilizada em processos que vão demorar algum tempo para finalizar a execução. Nesses casos, as tarefas são colocadas em uma fila (que para serem executadas posteriormente, liberando o usuário do sistema para outras tarefas. Exemplos de uso: Geração de relatórios, processamento de cadastros de mídias (auto índice de I/O):

![img](https://static.imasters.com.br/wp-content/uploads/2019/05/27152812/0_DOyIY8iAbbyZBR1p.png)Exemplo de [Work Queues na documentação RabbitMQ](https://www.rabbitmq.com/tutorials/tutorial-two-go.html)

### Publish/Subscribe –  Enviando mensagens para muitos destinatários

A diferença entre esse padrão e o anterior, é que no anterior trabalhamos apenas com uma queue (fila), e aqui trabalhamos com diversas queues.

Ao disparar a mensagem, o usuário não sabe qual queue ela vai ser enviada. Esse padrão ainda se ramifica para quatro tipos: **direct**, **topic**, **headers** e **fonout**.

Exemplos de uso: **chats**, **push notifications**, **logs**:

![img](https://static.imasters.com.br/wp-content/uploads/2019/05/27152903/0_ARsXkr6xG8RNLs_5.png)Exemplo de [Publish/Subscribe na documentação RabbitMQ](https://www.rabbitmq.com/tutorials/tutorial-three-go.html)

### Routing –  Seleção de qual(is) fila(s) sua mensagem vai pertencer usando uma característica chave

Nesse padrão, trabalha-se como no anterior, com o bônus de que o sender pode classificar as mensagens e direciona-las a uma fila específica.

Soluções que usam teoria de grafos como base são boas candidatas a esse padrão (olha a matemática aí de novo, minha gente). Exemplos de uso: pushs direcionados, paralelismo de tarefas para mesma ‘mensagem’, logs classificados.

![img](https://static.imasters.com.br/wp-content/uploads/2019/05/27152934/0_SiFdyPRqp_rmBtKm.png)Exemplo de [Routing na documentação RabbitMQ](https://www.rabbitmq.com/tutorials/tutorial-four-go.html)

### Topics – Classificação de uma mensagem por uma combinação de chaves

Aqui as coisas ficam interessantes. Nesse momento, o protagonista não são as filas, mas a mensagem, então a mensagem enviada pode ser incluída em mais de uma fila e processada de formas diferentes, simultaneamente.

Isso é possível através de uma lista de palavras chave que classificam nossa mensagem em filas diferentes! Vejo esse padrão muito ligado a deep learning e IA. Exemplos de uso: ‘tageamento’, classificação e distribuição de conteúdo e chats.

![img](https://static.imasters.com.br/wp-content/uploads/2019/05/27153013/0_W-BWd1qHb02-PozT.png)Exemplo de [Topics na documentação RabbitMQ](https://www.rabbitmq.com/tutorials/tutorial-five-go.html)

### RPC (Remote Procedure Call) –  Chamada de procedimento remoto: Comunicação entre apps, services ou apis usando filas

Esse padrão é usado para comunicação entre aplicações diferentes. Parece um pouco com o padrão Work queues, mas no caso do RPC, quem enviou a mensagem espera uma resposta de quem recebeu a mensagem. Te lembrou do protocolo HTTP?

Lembra, né? A diferença é que usando o RabbitMQ teremos uma camada a mais, que são as filas, para garantir que a nossa mensagem não se perca no meio do caminho.

As mensagem são alocadas nas filas, e lidas pelo server quando ele estiver disponível. Quando usamos HTTP, caso a aplicação no server tenha algum problema de comunicação, o cliente recebe um erro de timeout, por exemplo.

**Exemplos de uso**: persistência da aplicação.

![img](https://static.imasters.com.br/wp-content/uploads/2019/05/27153046/1_XDQFEyzO_xxJw-pRZ3S1XQ.png)Exemplo de comunicação HTTP simplificado

![img](https://static.imasters.com.br/wp-content/uploads/2019/05/27153112/0_zdrX1PGhbm1D-TvB.png)Exemplo de [RPC na documentação do RabbitMQ](https://www.rabbitmq.com/tutorials/tutorial-six-go.html)

Enfim, é um assunto muito amplo, com muitos tópicos que merecem uma série de artigos cada um. Se curtirem essa ideia, comentem aí embaixo que podemos fazer um exemplo para cada tipo de implementação, beleza?

Espero que esse artigo te ajude a entender um pouco sobre como funciona esse mundo das filas no RabbitMQ, e caso tenha alguma dúvida ou sugestão, deixe aí nos comentários e vamos trocar!

## Referências

- [Teoria das filas: entenda como funciona no cotidiano](https://www.cmtecnologia.com.br/teoria-das-filas/)
- [Teoria das filas](https://pt.wikipedia.org/wiki/Teoria_das_filas)
- [RabbitMQ Tutorials](https://www.rabbitmq.com/getstarted.html)