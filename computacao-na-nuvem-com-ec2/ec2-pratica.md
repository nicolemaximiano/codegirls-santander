🧩 Resumo da Aula — Computação na Nuvem com Amazon EC2
☁️ O que é o EC2?

O Amazon EC2 (Elastic Compute Cloud) é um serviço de computação em nuvem da AWS que oferece máquinas virtuais (instâncias) configuráveis com CPU, memória, armazenamento e rede.
Faz parte do modelo IaaS (Infraestrutura como Serviço), onde o usuário é responsável por gerenciar aplicações, dados e conexões.

🎯 Escolhendo a Instância EC2 Correta

As instâncias são classificadas conforme o tipo de carga de trabalho:
| Categoria                 | Foco Principal                                       | Exemplos    |
| ------------------------- | ---------------------------------------------------- | ----------- |
| **General Purpose**       | Uso geral (web servers, pequenos bancos de dados)    | A1, T2, M4  |
| **Compute Optimised**     | Alto desempenho de CPU                               | C4          |
| **Memory Optimised**      | Aplicações que exigem muita memória (ex: SAP, Spark) | R4, X1, z1d |
| **Accelerated Computing** | Machine Learning, gráficos, vídeo, IA                | P2, G3, F1  |
| **Storage Optimised**     | Alto throughput e armazenamento intenso              | H1, I3, D2  |

---

💸 Otimização de Recursos na AWS

Otimizar recursos significa melhorar o desempenho e reduzir custos.
Principais práticas:

- Otimizar custos e desempenho → ajustar recursos conforme necessidade.
- Desligar instâncias não utilizadas → em horários ociosos (noite/fins de semana).
- Remover recursos ociosos → liberar o que não está sendo usado.
- Escalabilidade vertical → aumentar ou reduzir capacidade (CPU, RAM, disco).
- Escalabilidade horizontal → adicionar mais instâncias para suportar maior demanda.
---

🛒 Tipos de Compra de Instâncias

Formas de adquirir instâncias conforme seu uso e orçamento:

| Tipo                          | Vantagem                         | Recomendado Para                          |
| ----------------------------- | -------------------------------- | ----------------------------------------- |
| **Sob Demanda (On-Demand)** ⏳ | Pagamento por hora de uso.       | Testes e cargas de curto prazo.           |
| **Instâncias Reservadas** 💰  | Mais baratas que as sob demanda. | Uso contínuo e previsível (ex: produção). |
| **Instâncias Spot** ⚡         | Até **90% mais baratas**.        | Processos que podem ser interrompidos.    |

--- 

🚀 Conclusão

- O EC2 oferece flexibilidade e escalabilidade para qualquer tipo de aplicação.
- A escolha correta da instância e do modelo de compra impacta diretamente no custo e desempenho.
- Monitorar, ajustar e desligar recursos ociosos são práticas essenciais de otimização em nuvem.
