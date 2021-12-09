![Nuvem AWS](https://d1.awsstatic.com/icons/header-icons/header-icon_%2caws-messaging.14b623533e7c8f46e5fd93a68acaf64f59f02619.png)

# Filas de mensagens

![Nuvem AWS](https://d1.awsstatic.com/Graphics/rule.8b3deaf243ba0c51cd290d635b55eb667aba05e2.png)

### Sistema de mensagens assíncronas para trabalhos em lote e aplicativos dissociados

[Comece a usar o Amazon SQS gratuitamente](https://console.aws.amazon.com/sqs/home)

#### [Benefícios das filas de mensagens](https://aws.amazon.com/pt/message-queue/benefits/)

#### [Recursos das filas de mensagens](https://aws.amazon.com/pt/message-queue/features/)

#### [Recursos da fila de mensagens](https://aws.amazon.com/pt/message-queue/resources/)

#### [Filas de mensagens da AWS: Amazon SQS](https://aws.amazon.com/sqs)

## O que é uma fila de mensagens?

Uma fila de mensagens é uma forma de comunicação assíncrona entre serviços usada em arquiteturas sem servidor e de microsserviços. As mensagens são armazenadas na fila até serem processadas e excluídas. Cada mensagem é processada uma única vez, por um único consumidor. As filas de mensagens podem ser usadas para dissociar processamento pesado, para armazenar trabalho em buffers ou lotes e para processar uniformemente picos de cargas de trabalho.

Veja a seguir vários recursos para ajudar você a entender melhor as filas de mensagens em um sentido mais amplo. Para saber mais sobre filas de mensagens na AWS, acesse o site do [Amazon Simple Queue Service (SQS)](https://aws.amazon.com/sqs).

[![webinar_decouple_and_scale_2017-06](https://d1.awsstatic.com/video-thumbs/Messaging/webinar_decouple_and_scale_2017-06.e93676bb96836ad52294c26840f20285219e5f05.png)33:27Assistir ao nosso webinar para compreender a função e os componentes do sistema de mensagens no projeto de aplicativos](https://www.youtube-nocookie.com/embed/UesxWuZMZqI)

## Fundamentos da fila de mensagens

Na arquitetura de nuvem moderna, os aplicativos são dissociados em componentes essenciais independentes, que são mais fáceis de desenvolver, implantar e manter. As filas de mensagens disponibilizam recursos de comunicação e coordenação para esses aplicativos distribuídos. As filas de mensagens podem simplificar bastante a codificação de aplicativos dissociados e aumentar a performance, a confiabilidade e a escalabilidade.

As filas de mensagens permitem que diferentes partes de um sistema se comuniquem e processem operações de forma assíncrona. Uma fila de mensagens disponibiliza um buffer leve que as armazena temporariamente, além de endpoints que permitem que os componentes de software estabeleçam conexão com a fila para o envio e o recebimento de mensagens. Geralmente, as mensagens são pequenas e podem ser itens, como solicitações, respostas, mensagens de erro, ou apenas informações. Para enviar uma mensagem, um componente chamado de produtor adiciona uma mensagem à fila. A mensagem é armazenada na fila até que outro componente chamado de consumidor recupere a mensagem e realize algo com ela.

![fila de mensagens](https://d1.awsstatic.com/product-marketing/Messaging/sqs_seo_queue.1dc710b63346bef869ee34b8a9a76abc014fbfc9.png)

Muitos produtores e consumidores podem usar a fila, mas cada mensagem é processada apenas uma vez, por um único consumidor. Por esse motivo, geralmente, esse padrão de sistema de mensagens é chamado de comunicação direta ou ponto a ponto. Quando uma mensagem precisa ser processada por mais de um consumidor, as filas de mensagens podem ser combinadas com um sistema de mensagens de publicação/assinatura em um padrão de projeto distribuído. Consulte "[O que é o sistema de mensagens de publicação/assinatura?](https://aws.amazon.com/pt/pub-sub-messaging/)" para obter detalhes, e acesse o site do [Amazon Simple Notification Service (SNS)](https://aws.amazon.com/pt/migration-acceleration-program/) para obter uma visão geral sobre o sistema de mensagens de publicação/assinatura na AWS.

## Próximas etapas

Comece a usar gratuitamente executando apenas três comandos simples.

[Comece a usar gratuitamente](https://console.aws.amazon.com/sqs/home)