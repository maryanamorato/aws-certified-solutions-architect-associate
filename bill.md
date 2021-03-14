# Billing

### [Simple Monthly Calculator](https://calculator.s3.amazonaws.com/index.html)
É basicamente isso aí mesmo, uma calculadora mensal, separada por recursos.

### [Pricing Calculator](https://calculator.aws/)
Você prepara um ambiente, colocando os recursos desejados e estimativa de uso, e ele lança uma estimativa de preço.

### [Total Cost of Ownership](https://www.investopedia.com/terms/t/totalcostofownership.asp#:~:text=The%20total%20cost%20of%20ownership%20(TCO)%20is%20the%20purchase%20price,its%20value%20is%20over%20time.&text=The%20item%20with%20the%20lower,value%20in%20the%20long%20run.)
O custo total de algo, considerando não apenas preço inicial, mas também de manutenção, operação, inatividade.

### [Budget](https://aws.amazon.com/aws-cost-management/aws-budgets/)
É um orçamento mesmo, você define um valor e eles te notificam antes ou depois de alcançá-lo, mas não vão bloquear a ultrapassagem. Em vez disso, você pode triggar uma ação como a aplicação de uma política do IAM que nega a criação de recursos na conta, por exemplo.

### [Cost Explorer](https://aws.amazon.com/pt/aws-cost-management/aws-cost-explorer/)
Relatórios de gastos e uso, gera até previsões. Dá para exportar, acessar usando API...

### [Consolidated Billing](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/consolidated-billing.html)
Cria uma fatura única com o Organizations, permite ver gastos individuais e agregados. Descontos nas categorias RIs e Saving Plans do EC2.

### [Cost Allocation Tags](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/cost-alloc-tags.html)
Uso de tags (podem ser criadas automaticamente ou personalizadas) para acompanhar grupos lógicos de forma independente no Cost Explorer

### [AWS Marketplace](https://aws.amazon.com/marketplace)
Catálogo personalizado que oferece diversas opções de assinatura.