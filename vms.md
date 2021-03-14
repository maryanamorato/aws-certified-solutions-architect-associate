# Compute

### [EC2](https://aws.amazon.com/ec2/faqs/)
VMs que podem ser on-demand, Spots (sobras? Não é muito confiável mas é mais barato e tão eficiente quanto a Standard), você pode se comprometer a utilizar uma quantidade específica (Saving Plans) ou uma configuração especifica (Instâncias Reservadas (tem a padrão e a conversível (mais flexivel e mais cara))) e ganhar desconto!

Você pode também reservar uma instância a nível de hardware (Instâncias Dedicadas), só para você ou até um host só seu (Host Dedicado), onde você pode inclusive adicionar suas licenças. Isso geralmente é usado quando se tem tretas de conformidade.

Ao hibernar uma instância, você economiza. Se você armazenar no EBS, S3 e tal, você pode persistir os dados mesmo terminando uma instância.
Um grupo de segurança do EC2 atua como Firewall controlando o tráfego.

### [EC2 Auto Scaling](https://aws.amazon.com/ec2/autoscaling/faqs/)
Criado para mudar a capacidade, iniciar ou encerrar automaticamente instâncias do Amazon EC2, garantindo disponibilidade do número correto de instâncias com a configuração ideal para processar as workloads, além de substituir instâncias não-íntegras. Dá suporte a algumas políticas que o Auto Scaling padrão não daria, mas ainda precisaria dele para usar escalabilidade preditiva (examina histórico de tráfego e prevê mudanças usando ML). Recebe configurações de execução, que seria um modelo usado para a criação das novas instâncias.

### [AWS Lambda](https://aws.amazon.com/lambda/faqs/)
Permite rodar código sem ter um servidor! Inclusive você nem pode acessar o server onde ele roda. Suas funções também precisam ser serveless. Código e estado persistente é armazenado no S3 ou outro storage.

### [Fargate](https://aws.amazon.com/fargate/faqs/)
Permite rodar containers sem ter um servidor! Fully-managed e on-demand. Caso precise de acesso à maquina que roda, o ideal seria um EC2 mesmo.

### [Amazon Lightsail](https://aws.amazon.com/lightsail/faq/)
Um EC2 levinho e mais barato, mas menos personalizável. Ele tem muita coisa gerenciada, ao contrário do EC2. Existe um botão de "Upgrade to EC2".  

### [AWS Elastic Beanstalk](https://aws.amazon.com/elasticbeanstalk/faqs/)
Servidor codebased. Você bota o app e ele administra capacidade, balanceamento de carga, autoscaling e integridade. Suporta Java, .NET, PHP, Node.js, Python, Ruby, Go e Docker. Armazena arquivos e logs no S3.

### [AWS Batch](https://aws.amazon.com/batch/faqs/)
Processamento em lote, tipo filas. Você lança o script e ele gerencia o resto, usando EC2 (Spot) e Fargate (orquesta containers de forma elástica). Evita ociosidade e permite deslocamento da carga de trabalho para horários mais baratos. É grátis, só se paga o EC2/Fargate.