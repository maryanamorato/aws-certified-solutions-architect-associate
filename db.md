
# Database

### [Throughput](https://www.intel.com.br/content/www/br/pt/support/articles/000026190/wireless.html)
Taxa em que os dados são transmitidos com êxito.

### [Database Migration Service (DMS)](https://aws.amazon.com/dms/faqs/)
Basicamente migração de bancos de dados.

### [RDS](https://aws.amazon.com/rds/faqs/)
Gerenciamento que facilita/automatiza tarefas de bancos relacionais (MySQL, SQL Server, MariaDB, Oracle, Postgres). Pode ser usado no on-premise com VMware ou Outposts, mas logs e backup ficam na nuvem. 

### [Aurora](https://aws.amazon.com/rds/aurora/faqs/)
Gerenciado pelo RDS. Compatível com MySQL e Postgres! Eficiente, seguro. Inclui replicação.

### [DynamoDB](https://aws.amazon.com/dynamodb/faqs/)
Não-relacional! Inclui replicação. Leituras podem ser:
* Eventualmente consistentes -> Pode não refletir resultados automaticamente;
* Fortemente consistentes -> Retorna tudo;
* ACID -> Garantias de integridade adicionais.

### [ElastiCache](https://aws.amazon.com/elasticache/faqs/)
Cache para o RDS e DynamoDB. Resiliente etc.. Compatível com Redis e Memcached. Cada node seria uma instância do serviço, enquanto um shard seria vários nodes (com um primário) e um cluster vários shards.

### [Redshift](https://aws.amazon.com/redshift/faqs/)
Mucho dado. Bom pra BI, dentre outras razões pelo armazenamento colunar. Separa computação e armazenamento (RA3 nodes), o que dá mais controle na escalação. Tem o spectrum, que tem a inteligência de escalar conforme se recebe os dados. Tam ém tem o AQUA, um cache distribuído acelerado com base em hardware, que permite processamento (computação) mesmo em cache. Já é replicado também.

### [Neptune](https://aws.amazon.com/neptune/faqs/)
Consultas SQL gráficas, como recomendação e proximidade.

### [QLDB](https://aws.amazon.com/qldb/faqs/)
Ledger/Livro-Razão (registro seguros de transações financeiras, tipo btc). Imutável.

### [DocumentDB](https://aws.amazon.com/documentdb/faqs/)
(MongoDB) Suporte a workloads.

### [KeySpaces](https://aws.amazon.com/keyspaces/faqs/)
(Cassandra) Suporte a workloads.

### [EMR](https://aws.amazon.com/emr/faqs/)
Webservice de processamento de muitos dados, como indexação da web, mineração de dados, análise de arquivos de log, machine learning e análise financeira.
