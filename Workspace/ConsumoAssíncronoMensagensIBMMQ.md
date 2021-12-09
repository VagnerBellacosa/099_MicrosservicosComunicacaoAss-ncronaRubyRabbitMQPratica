# Consumo assíncrono de mensagens do IBM MQ

O consumo assíncrono usa um conjunto de extensões da Message Queue Interface (MQI), as chamadas MQI MQCB e MQCTL, que permitem que um aplicativo MQI seja escrito para consumir mensagens de um conjunto de filas. As mensagens são entregues ao aplicativo chamando uma 'unidade de código' identificada pelo aplicativo passando a mensagem ou um token que representa a mensagem.

No mais direto dos ambientes de aplicativos, a unidade de código é definida por um ponteiro de função, no entanto, em outros ambientes, a unidade de código pode ser definida por um nome de programa ou módulo.

No consumo assíncrono de mensagens, os termos a seguir são usados:

- Consumidor de mensagens

  Uma construção de programação que permite definir um programa, ou função, a ser chamado com uma mensagem quando uma que corresponda ao requisito dos aplicativos se torna disponível.

- Manipulador de eventos

  Uma construção de programação que permite definir um programa ou função para chamar quando um evento assíncrono, como quiesce do gerenciador de filas, ocorre.

- Retorno de chamada

  Um termo genérico usado para fazer referência a uma rotina do Consumidor de mensagens ou do Manipulador de eventos.

Consumo assíncrono pode simplificar o design e a implementação de novos aplicativos, principalmente aquelas que processam diversas filas de entrada ou assinaturas. No entanto, se você estiver usando mais de uma fila de entrada e estiver processando as mensagens na sequência de prioridade, a sequência de prioridade será observada independentemente em cada fila. Pode ser que você obtenha mensagens de prioridade baixa de uma fila antes de mensagens de prioridade alta de outra. A ordem das mensagens entre várias filas não é garantida. Observe também que se você usar saídas de API, poderá precisar mudá-las para incluir as chamadas de MQCB e MQCTL.

As ilustrações a seguir fornecem um exemplo de como é possível usar essa função.

[Figura 1](https://www.ibm.com/docs/pt-br/ibm-mq/9.0?topic=ssfksj-9-0-0-com-ibm-mq-dev-doc-q023050--htm#q023050___q023050_1) mostra um aplicativo multiencadeado consumindo mensagens a partir de duas filas. O exemplo mostra todas as mensagens que estão sendo entregues a uma única função.

Figura 1. Aplicativo padrão acionado por mensagens consumindo de duas filas

![Esse fluxo de amostra mostra um aplicativo multiencadeado consumindo mensagens de duas filas. O exemplo mostra todas as mensagens sendo entregues a uma única função.](https://www.ibm.com/docs/pt-br/SSFKSJ_9.0.0/com.ibm.mq.dev.doc/q023050a.gif)

![[z/OS]](https://www.ibm.com/docs/pt-br/SSFKSJ_9.0.0/com.ibm.mq.dev.doc/ngzos.gif)No z/OS, o encadeamento de controle principal deve emitir uma chamada MQDISC antes de ser finalizado. Isso permite que quaisquer encadeamentos de retorno de chamada finalizem e liberem recursos do sistema.

[Figura 2](https://www.ibm.com/docs/pt-br/ibm-mq/9.0?topic=ssfksj-9-0-0-com-ibm-mq-dev-doc-q023050--htm#q023050___q023050_2)Esse fluxo de amostra mostra um aplicativo de encadeamento único consumindo mensagens de duas filas. O exemplo mostra todas as mensagens que estão sendo entregues a uma única função.

A diferença do caso assíncrono é que o controle não retornará para o emissor de MQCTL até que todos os consumidores tiverem se desativado; ou seja, um consumidor emitiu uma solicitação MQCTL STOP ou o gerenciador de filas efetua quiesce.

Figura 2. Aplicativo acionado por mensagens de encadeamento único consumindo de duas filas

![Esse fluxo de amostra mostra um aplicativo de encadeamento único consumindo mensagens de duas filas. O exemplo mostra todas as mensagens sendo entregues a uma única função.](https://www.ibm.com/docs/pt-br/SSFKSJ_9.0.0/com.ibm.mq.dev.doc/q023050b.gif)

**Tópico pai:**

[Mensagens do IBM MQ](https://www.ibm.com/docs/pt-br/SSFKSJ_9.0.0/com.ibm.mq.dev.doc/q022860_.htm)