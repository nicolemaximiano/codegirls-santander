☁️💻 Computação na Nuvem com Amazon EC2

O módulo foca em Computação na Nuvem com EC2, Armazenamento na Nuvem, Gerenciamento de Instâncias EC2 e Otimização de Recursos na AWS.

🖥️ 1. O que são Instâncias Amazon EC2?

O Amazon EC2 (Elastic Compute Cloud) fornece máquinas virtuais na nuvem da AWS, oferecendo capacidade de computação escalável e flexível.
As instâncias podem executar Windows ou Linux e são compostas por:

💡 CPU, Memória, Disco, Rede e Sistema Operacional

No modelo de nuvem, o EC2 é classificado como IaaS (Infraestrutura como Serviço).
Nossa responsabilidade inclui os aplicativos, dados e conexões utilizados nas instâncias.

🎯 2. Escolhendo a Instância EC2 Correta

A escolha da instância correta é crucial para garantir eficiência, escalabilidade e economia nos gastos com nuvem.
As instâncias são categorizadas conforme seu propósito:

🏷️ Categoria	🧠 Descrição	⚙️ Exemplos (Séries)
General Purpose	Servidores de aplicação principal e propósito geral. Ex: ARM based core e custom silicon; Web servers pequenos e DBs pequenos	A1, T2, M4
Compute Optimised	Otimizadas para aplicações intensivas em CPU e bancos de dados (DBs)	C4
Memory Optimised	Otimizadas para aplicações e bancos de dados (DBs) intensivos em memória (RAM). Ex: Xtreme RAM para SAP/Spark; High Compute e High Memory – Gaming	R4, X1, z1d
Accelerated Computing	Otimizadas para processamento, Machine Learning, gráficos intensivos, vídeo, streaming e hardware acceleration	P2, G3, F1
Storage Optimised	Otimizadas para alto throughput de disco, clusters de Big Data, IOPS e Data Warehousing	H1, I3, D2
💸 3. Otimização de Recursos na AWS

Otimizar recursos na AWS está diretamente ligado à redução de custos e melhoria de desempenho.
Confira as principais estratégias:

⚙️ Estratégia de Otimização	📝 Descrição
Otimização de Custos e Desempenho	Melhorar o desempenho do sistema resulta em economia e ganho de eficiência na solução em nuvem.
Desligando Instâncias Não Utilizadas 🛑	Em ambientes de desenvolvimento, teste ou treinamento, desligar instâncias fora do horário de uso reduz custos.
Remover Recursos Ociosos/Não Utilizados 🗑️	Recursos ociosos continuam gerando gastos — como alugar um carro e deixá-lo na garagem.
Escalabilidade (Horizontal e Vertical) 📈📉	Ajustar os recursos conforme a demanda — pode ser feito de forma manual ou automática.
Escalabilidade Vertical	Aumenta ou reduz capacidade em um mesmo nó (vCPUs, memória, storage, rede).
Escalabilidade Horizontal	Adiciona novos recursos (ex: novas instâncias) para suportar o aumento da carga.
🛒 4. Tipos de Compra de Instâncias (Para Otimização)

Existem diferentes formas de adquirir instâncias EC2, cada uma com vantagens e desvantagens relacionadas a custo, disponibilidade e flexibilidade:

💳 Tipo de Compra	✅ Vantagens	⚠️ Desvantagens / Recomendação
1. Sob Demanda (On-Demand) ⏳	Pagamento a uma taxa fixa por hora.	Ideal para cargas de trabalho irregulares de curto prazo que não podem ser interrompidas. Também recomendadas para testes e desenvolvimento.
2. Instâncias Reservadas 💰	Mais baratas que as sob demanda.	Exigem compromisso de uso (pagamento anual). Pouco vantajosas se a instância não for usada frequentemente.
3. Instâncias Spot ⚡	Oferecem descontos de até 90%.	Podem ser encerradas pela AWS a qualquer momento, com aviso prévio de 2 minutos.
🚀 Resumo

EC2 oferece infraestrutura elástica e sob demanda.

Escolher o tipo certo de instância e compra garante performance e economia.

A otimização contínua é a chave para manter custos baixos e sistemas eficientes na nuvem.
