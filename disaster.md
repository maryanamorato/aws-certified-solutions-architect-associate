
# [Disaster Recovery](https://docs.aws.amazon.com/wellarchitected/latest/reliability-pillar/plan-for-disaster-recovery-dr.html)

### Recovery Time Objective (RTO)
Objetivo do tempo de recuperação. Seria o atraso máximo aceitável entre a interrupção do serviço e a sua restauração.

### Recovery Point Objective (RPO)
Objetivo do ponto de recuperação. Seria o tempo máximo aceitável desde o último ponto de recuperação de dados. 

Ao projetar uma estratégia de várias regiões (previnindo falhas em AZ) para sua carga de trabalho, você deve escolher uma das seguintes estratégias

* ####  Backup & Restore (RPO em horas, RTO em 24 horas ou menos)

* #### Pilot Light (RPO em minutos, RTO em horas)
	Mantenha uma versão mínima de um ambiente com os elementos principais mais críticos do seu sistema na região de DR.

* #### Warm Standby (RPO em segundos, RTO em minutos)
	Mantenha uma versão reduzida de um ambiente totalmente funcional sempre em execução na região de DR.

* ####  Active-active (RPO nenhum, RTO em segundos)
	Workloads implantados em várias regiões da AWS. Essa estratégia requer que você sincronize os dados entre as regiões que está usando. Para recuperar, serviços como o Amazon Route 53 ou o Global Accelerator vão rotear o tráfego dos usuários ao local da carga de trabalho íntegra.