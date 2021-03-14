# Storage

### [Amazon S3](https://aws.amazon.com/s3/faqs/)
Armazenamento de objetos, que são disponibilizados por uma API. Não é possível editar os arquivos, somente fazer download e upload. Standard, Intelligent-Tiering (adapta-se aos padrões), Standard-Infrequent, 1 Zone-Infrequent, Outposts (usado em S3 on-premises). Cross-Replication permite cópia automática entre buckets, mas caso algum objeto seja deletado permanecerá no bucket reserva.

### [Amazon S3 Glacier](https://aws.amazon.com/glacier/faqs/)
Glacier, Glacier Deep Archive (geralmente usado para cumprimr conformidade). Demoram para recuperar os arquivos.

### [Amazon EBS](https://aws.amazon.com/ebs/faqs/)
Armazenamento em bloco (HD), projetado para uso com EC2. Apesar do "Elastic", ele tem seu tamanho alterado manualmente. Mesmo ao excluir a EC2, ele continua ali. É possível criar Snapshots, que são como linhas de base ou "templates" para novos volumes.

### [Amazon EFS](https://aws.amazon.com/efs/faq/)
Armazenamento de arquivos, projetado para uso com EC2. Tem uma interface de sistema de arquivos, semântica de acesso (consistência forte ou bloqueio de arquivos) e permite acesso simultâneo em milhares de EC2.

### [AWS Storage Gateway](https://aws.amazon.com/storagegateway/faqs/)
Permite acesso local a armazenamento em nuvem, com protocolos como iSCSI, SMB e NFS. Possui cache local, reduzindo latência. Geralmente usado para consultar backups e oferecer aos aplicativos locais acesso a dados armazenados na AWS.

### [AWS DataSync](https://aws.amazon.com/datasync/faqs/)
Transferência de dados online entre on-premise e nuvem ou entre serviços da AWS. 

### Amazon FSX
Armazenamento de arquivos, que integra-se com o [Lustre](https://aws.amazon.com/fsx/lustre/faqs/) ou o [Windows File Service](https://aws.amazon.com/fsx/windows/faqs/), que são sistemas de arquivos (com pastas compartilhadas e tal). Ṕara o WFS, dá uma gama de recursos administrativos (AD). Pode, inclusive, ser acessado de máquinas não-Windows.
Para o Lustre, elimina a complexidade de configuração e gerenciamento. Usado quando a velocidade é importante, como ML, processamento de vídeo etc.

### [AWS Snowball](https://aws.amazon.com/snowball/faqs/)
Dispositivos robustos e seguros para utilizar os recursos de armazenamento e computação da AWS em ambientes tipo navios e transferir dados deles para a AWS.