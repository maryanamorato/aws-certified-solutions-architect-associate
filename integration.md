#  Messaging and Integration

### [Amazon SQS](https://aws.amazon.com/sqs/faqs/)
Serviço de fila de mensagens entregues com um SDK. Bem configurável no que diz respeito a envio, que pode ser paralelo ou sequencial, em qualquer dia.

### [Amazon SNS](https://aws.amazon.com/sns/faqs/)
Prático e interno. Usado para enviar texto plano por email, SMS ou HTTP. É geralmente triggado por outros serviços. Cobranças ou códigos de confirmação por email são bons exemplos. Segue o paradigma pub-sub.

### [Amazon SES](https://aws.amazon.com/ses/faqs/)
Voltado para Marketing. Parecido com o Sendgrid! Permite envio de emails HTML, podendo-se customizar domínio, criar templates, monitorar reputação etc.

### [MQ](https://aws.amazon.com/amazon-mq/features/#FAQs)
Integrável a outros serviços de mensageria.

### [Step Functions](https://aws.amazon.com/step-functions/faqs/)
Realiza coordenação de funções dentro de uma aplicação.

### [Amazon Kinesis](https://aws.amazon.com/kinesis/streams/faqs/)
Coleta (SDK), processa e analisa streaming de dados em tempo real. Dados são criptografados e podem ser acessados por meio de API
	* Video Streams -> Dados de vídeo que podem ser usados para monitorar segurança, detecção de faces.. Pode ser integrado com o Amazon Recognition Video;
	* Data Streams -> Recebe dados como como clickstreams de sites, streams de eventos de BDs, transações financeiras, feeds de mídia social, logs e eventos de rastreamento de local (Extract);
	* Data Analytics -> Atua junto com o Apache Flink (faz processamento de dados), facilitando a integração deste com outros serviços da AWS (Transform);
	* Data Firehose -> Envia os dados de Streaming p serviços internos como S3, Redshift, Elasticsearch; serviços externos como MongoDB e Splunk ou até mesmo endpoints HTTP (Load).
