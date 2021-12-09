# Introdução ao RabbitMQ

24 NOV, 2021

## Introdução

Para quem não conhece, o RabbitMQ é um serviço de mensageria que utiliza o protocolo AMQP (Advanced Message Queuing Protocol) para transporte de dados. Esse protocolo nos permite trabalhar com envio de mensagens assíncronas.

Existem algumas formas de se implementar ele, e hoje irei abordar as três mais conhecidas: Workers, Pub/Sub e RPC (Remote Procedure Call). Abaixo, você tem uma breve introdução de cada uma delas:

## Workers

Essa implementação é utilizada quando você tem uma alta demanda de processamento bloqueante, como: processamento de uma fila de vídeos (que utiliza muito I.O), update em massa em uma carga de dados (para não deixar o seu usuário esperando o retorno), etc. Abaixo, você tem uma imagem que demonstra como ele funciona:

![img](https://static.imasters.com.br/wp-content/uploads/2018/05/30171403/0_Tg4DEJG-UPWVjrWT.png)

Analisando essa imagem, você tem:

- **p**: seria a sua aplicação. Pode ser uma Api, um site, algo que envie a requisição para sua fila
- **blocos em vermelho**: seria a sua fila do RabbitMQ
- **C1 e C2**: seus workers

## Publish/Subscribe (pub/sub)

O pub/sub é utilizado em muitos cenários do nosso dia dia, como: push notification, chat, envio de mensagens, etc. Abaixo, você pode ver três formas de se implementar ele:

- **direct:** envio direto de mensagem através de uma referência
- **topic:** em muitos aplicativos você pode assinar um tópico e aguardar mensagens sobre ele (push notification)
- **fanout:** seria o envio de mensagens em massa, como um broadcast

## RPC (Remote Procedure Call)

Esse modelo é utilizado na comunicação entre aplicações desenvolvidas em diferentes tecnologias. Imagine o seguinte cenário: Um app desenvolvido em Node.js precisa fazer requisições em uma API .NET Core, mas mesmo que o server caia, essas requisições não podem ser perdidas.

Tendo esse cenário anterior em mente, vamos analisar a imagem abaixo:

![img](https://static.imasters.com.br/wp-content/uploads/2018/05/30171448/0_GXsBC7YO805FIRKD_.png)RabbitMQ RPC

- **c (client):** seria a nossa aplicação Node.js; estamos enviando três informações para o exchange: replay_to (fila que eu irei aguardar), correlation_id= minha referencia, como eu posso ser localizado, e os dados em buffer que eu quero enviar para minha fila
- **rpc_queue:** essa seria a fila que irá receber os dados do exchange e enviará para o server
- **server:** seria o projeto .NET Core. Receberá os dados, realizará as regras e devolverá para a fila que veio no reply_to
- **reply_to:** retornará os dados processados junto com o correlation_id

Esse seria o fluxo básico de utilização do modelo RPC do RabbitMQ.

Bom, esse foi somente uma artigo de introdução ao RabbitMQ. Nós próximos criarei alguns exemplos utilizando ele com Node.js. Espero que tenham gostado e até um próximo artigo, pessoal.