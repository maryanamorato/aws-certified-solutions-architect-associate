# Concepts
Alguns conceitos que caem bastante em diversos contextos:


### [CQRS](https://docs.aws.amazon.com/whitepapers/latest/modern-application-development-on-aws/command-query-responsibility-segregation.html)
Command Query Responsability Segregation, significa separar a responsabilidade de escrita e leitura de seus dados.

 ### [Upfront Cost]([https://www.masterclass.com/articles/upfront-cost-definition#what-is-an-upfront-cost](https://www.masterclass.com/articles/upfront-cost-definition#what-is-an-upfront-cost))
 Quantia inicial de dinheiro investido em algo.

 ### [Horizontal (out) / Vertical (up) Scaling](https://www.section.io/blog/scaling-horizontally-vs-vertically/)
 Horizontal se refere a criação de mais instâncias para suportar a demanda. Vertical seria adicionar mais poder (CPU, RAM) às instâncias existentes. Seria tipo quantidade x qualidade.

### [Responsabilidade da AWS](https://aws.amazon.com/pt/compliance/shared-responsibility-model/)
“Segurança da nuvem”: operar SOs do host, a camada de virtualização e a segurança física dos DCs, ou seja, proteger a infraestrutura que executa os serviços, composta por hardware, software, redes e instalações que executam os serviços.

### [Responsabilidade do cliente](https://aws.amazon.com/pt/compliance/shared-responsibility-model/)
"Segurança na nuvem”: Um serviço de IaaS, por exemplo, exige que o cliente execute a configuração e gerenciamento da segurança (como o firewall da AWS (grupo de segurança)), do SO (incluindo atualizações e patches de segurança). Para serviços abstraídos, como o S3 e DynamoDB, são responsáveis pelos dados (incluindo criptografia) e uso do IAM para aplicar permissões.

### [SLA](https://aws.amazon.com/pt/legal/service-level-agreements/)
Acordo de nível de serviço, tipo um "Elimina 99,9999% dos germes!".

### [Well Architected Framework](https://aws.amazon.com/pt/architecture/well-architected/)
Analisa workloads em relação a boas práticas, ajudando a criar infraestruturas de aplicativos seguras, resilientes, eficientes e de alta performance.