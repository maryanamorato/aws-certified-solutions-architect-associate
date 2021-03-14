# Containers

### [ECS](https://aws.amazon.com/ecs/faqs/)
 Orquestrador de containers. Usando junto ao Fargate, você não precisa criar as EC2, o fargate lidaria com isso (serverless).  

### [EKS](https://aws.amazon.com/eks/faqs/)
Feito para integrar com um cluster do Kubernetes (um orquestrador de containers). É mais prático que o ECS caso queira migrar de nuvem. Tem que criar as EC2 também, ou usar node-groups (self-managed: permitem criação/exclusao) ou ainda o Fargate (fully-managed).

### [ECR](https://aws.amazon.com/ecr/faqs/)
Repositório de imagens (storage e deploy).