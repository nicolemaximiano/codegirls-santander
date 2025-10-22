Computação na Nuvem com EC2 ☁️💻

O módulo foca em Computação na Nuvem com EC2 , Armazenamento na Nuvem , Gerenciamento de instâncias EC2 e Otimização de recursos na AWS.

1. O que são Instâncias Amazon EC2? 🖥️

EC2 (Elastic Compute Cloud) são as máquinas virtuais fornecidas pela AWS , oferecendo capacidade de computação na cloud.
Podem utilizar sistemas operacionais Windows ou Linux.

Uma instância EC2 é composta por:
CPU, Memória, Disco, Rede e Sistema Operacional 

No modelo Cloud, a EC2 é classificada como IaaS (Infraestrutura como Serviço).

Nossa responsabilidade sobre a EC2 no modelo IaaS seria com os aplicativos, dados e conexões que realizamos.

2. Escolhendo a Instância EC2 Correta 🎯

A escolha da instância correta é crucial para garantir eficiência, escalabilidade e economia nos gastos com nuvem. As instâncias são categorizadas com base em seu propósito:

| Categoria                 | Descrição                                                                                                                                          | Exemplos (Séries) |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------- |
| **General Purpose**       | Servidores de aplicação principal e propósito geral. Ex: ARM based core e custom silicon; Web servers pequenos e DBs pequenos                      | A1, T2, M4        |
| **Compute Optimised**     | Otimizadas para aplicações intensivas em CPU e bancos de dados (DBs)                                                                               | C4                |
| **Memory Optimised**      | Otimizadas para aplicações e bancos de dados (DBs) intensivos em memória (RAM). Ex: Xtreme RAM para SAP/Spark; High Compute e High Memory – Gaming | R4, X1, z1d       |
| **Accelerated Computing** | Otimizadas para processamento, Machine Learning, gráficos intensivos, vídeo e streaming, e hardware acceleration                                   | P2, G3, F1        |
| **Storage Optimised**     | Otimizadas para alto throughput de disco, clusters de Big Data, IOPS e Data Warehousing                                                            | H1, I3, D2        |

3. Otimização de Recursos na AWS 💸
Otimizar recursos na AWS está diretamente relacionado a poupar custos.

| Estratégia de Otimização                         | Descrição                                                                                                                                                                                                |
| ------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Otimização de Custos e Desempenho**            | Mesmo otimizar um recurso computacional para melhorar o desempenho do sistema resulta em economia, pois isto traz ganho para a solução na nuvem                                                          |
| **Desligando Instâncias Não Utilizadas 🛑**      | Em ambientes de desenvolvimento, testes ou treinamento, instâncias que não são usadas à noite ou nos fins de semana podem ser desligadas. Uma menor utilização implica diretamente em economia de custos |
| **Remover Recursos Ociosos/Não Utilizados 🗑️**  | Recursos ociosos, parados no ambiente, geram gastos. Seria como alugar um carro e deixá-lo na garagem                                                                                                    |
| **Escalabilidade (Horizontal e Vertical) 📈/📉** | Executar o scale de recursos para processar os workloads em determinados momentos. Pode ser manual ou automático                                                                                         |
| **Escalabilidade Vertical**                      | Significa acrescentar ou reduzir capacidade de um recurso em um mesmo nó, alterando vCPUs, memória, storage, rede de uma instância                                                                       |
| **Escalabilidade Horizontal**                    | Aumentar o número de recursos, como adicionando mais um disco rígido ou mais uma instância para suportar a aplicação                                                                                     |

4. Tipos de Compra de Instâncias (Para Otimização) 🛒
   
| Tipo de Compra                   | Vantagens                                                                         | Desvantagens / Recomendação                                                                                                                                                                 |
| -------------------------------- | --------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1. Sob Demanda (On-Demand) ⏳** | Pagamento a uma taxa fixa por hora.                                               | Recomendadas para aplicações com cargas de trabalho irregulares de curto prazo que não podem ser interrompidas. Também adequadas para uso durante o teste e desenvolvimento de aplicativos. |
| **2. Instâncias Reservadas 💰**  | Costumam ser mais baratas que as instâncias sob demanda.                          | É preciso pagar o ano inteiro de uso, o que é uma desvantagem para quem não precisa usar a instância com frequência.                                                                        |
| **3. Instâncias SPOT ⚡**         | Garantem disponibilidade das aplicações sob demanda com descontos de até **90%**. | Podem ser encerradas pela AWS a qualquer momento, com um aviso de dois minutos.                                                                                                             |

