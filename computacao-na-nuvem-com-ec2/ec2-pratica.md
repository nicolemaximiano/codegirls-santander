# Módulo 2 – Computação na Nuvem com EC2

📚 **Resumo:** Este repositório contém o resumo dos principais tópicos abordados no Módulo 2 da Formação AWS Cloud Foundations, com foco em **Computação na Nuvem (EC2)**, **Armazenamento (S3 e EBS)** e **Otimização de Recursos na AWS**.

---

## 📑 Sumário
1. [Computação na Nuvem – Amazon EC2 🖥️](#-1-computação-na-nuvem--amazon-ec2-️)
2. [Armazenamento na Nuvem – S3 e EBS 🗄️](#-2-armazenamento-na-nuvem--s3-e-ebs-️)
3. [Otimização de Recursos e Custos 💰](#-3-otimização-de-recursos-e-custos-)
4. [Conclusão 🚀](#-conclusão-)

---

## 🖥️ 1. Computação na Nuvem – Amazon EC2

O **Amazon EC2 (Elastic Compute Cloud)** é um serviço de **computação sob demanda** que oferece **máquinas virtuais (instâncias)** configuráveis.  
Essas instâncias fazem parte do modelo **IaaS (Infraestrutura como Serviço)**, e o usuário é responsável por **aplicativos, dados e conexões**.

Cada instância EC2 é composta por:
> 💡 **CPU, Memória, Disco, Rede e Sistema Operacional**

### 🔹 Tipos de Instâncias EC2

| Categoria | Descrição | Exemplos (Séries) |
|------------|------------|-------------------|
| **General Purpose** | Uso geral: servidores web, pequenos bancos de dados | A1, T2, M4 |
| **Compute Optimised** | Foco em alto desempenho de CPU | C4 |
| **Memory Optimised** | Ideal para aplicações que exigem muita memória (SAP, Spark, etc.) | R4, X1, z1d |
| **Accelerated Computing** | Machine Learning, gráficos e processamento pesado | P2, G3, F1 |
| **Storage Optimised** | Alto throughput de disco, Big Data e Data Warehousing | H1, I3, D2 |

---

## 🗄️ 2. Armazenamento na Nuvem – S3 e EBS

### 🧱 **Amazon S3 (Simple Storage Service)**
O **S3** é um serviço de **armazenamento de objetos** seguro, escalável e altamente durável.  
Ideal para armazenar grandes volumes de dados e acessá-los de forma global.

| Classe | Frequência de Acesso | Objetivo Principal |
|--------|----------------------|--------------------|
| **S3 Standard** | Frequente | Alta disponibilidade e performance (dados acessados regularmente). |
| **S3 Standard-IA** | Infrequente | Menor custo, acesso imediato quando necessário. |
| **S3 One Zone-IA** | Infrequente | Mais econômico, porém limitado a uma Zona de Disponibilidade. |
| **S3 Glacier / Deep Archive** | Raro | Armazenamento de baixo custo para arquivamento e backup de longo prazo. |

> 🔁 **Lifecycle Policies:** permitem mover objetos automaticamente entre classes, otimizando custos.

---

### 💽 **Amazon EBS (Elastic Block Store)**
O **EBS** fornece **armazenamento em blocos persistente** para instâncias EC2.  
Funciona como um **disco rígido virtual** anexado a uma instância.

- 📦 Permite expansão rápida de capacidade.  
- 🔒 Alta confiabilidade e persistência.  
- 🧰 Usos comuns: **bancos de dados (MySQL, Oracle)**, **aplicações web** e **logs de sistema**.

---

## 💰 3. Otimização de Recursos e Custos

Otimizar recursos significa **aumentar eficiência e reduzir gastos**.  
A AWS oferece diversas estratégias para isso:

| Estratégia | Descrição |
|-------------|------------|
| **Desligar instâncias não utilizadas 🛑** | Em ambientes de Dev/Test/Treinamento, desligar instâncias fora do horário de uso gera economia. |
| **Remover recursos ociosos 🗑️** | Evitar custos com recursos parados e não utilizados. |
| **Escalabilidade Vertical ⬆️** | Aumentar ou reduzir recursos (CPU, memória, storage) no mesmo nó. |
| **Escalabilidade Horizontal ➡️** | Adicionar novas instâncias para dividir a carga e suportar picos de demanda. |

---

### 🛒 **Tipos de Compra de Instâncias EC2**

| Tipo de Compra | Vantagem | Recomendação |
|----------------|-----------|---------------|
| **Sob Demanda (On-Demand) ⏳** | Pagamento por hora de uso. | Ideal para testes e workloads de curto prazo. |
| **Instâncias Reservadas 💰** | Mais baratas que as sob demanda. | Recomendadas para uso contínuo e previsível. |
| **Instâncias Spot ⚡** | Até **90% de desconto**. | Indicadas para tarefas flexíveis e não críticas. |

---

## 🚀 Conclusão

O **Módulo 2** da Formação AWS Cloud Foundations apresenta os conceitos essenciais de **computação e armazenamento na nuvem**, destacando:

- 🧠 **EC2**: infraestrutura escalável e flexível.  
- 💾 **S3 e EBS**: soluções robustas e seguras para armazenamento.  
- 💸 **Otimização de recursos**: reduzir custos sem perder desempenho.  

> ⚡ *A base da nuvem AWS é compreender como escalar, otimizar e gerenciar recursos de forma inteligente e econômica.*

---


