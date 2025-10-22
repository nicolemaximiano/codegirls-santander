# ☁️ Módulo 2 – Computação na Nuvem com EC2  

📚 **Resumo:**  
Este repositório contém o resumo dos principais tópicos abordados no Módulo 2, com foco em **Computação na Nuvem (EC2)**, **Armazenamento (S3 e EBS)** e **Otimização de Recursos na AWS**.

---

## 📑 Sumário
1. [Computação na Nuvem – Amazon EC2 🖥️](#-1-computação-na-nuvem--amazon-ec2)
2. [Armazenamento na Nuvem – S3 e EBS 🗄️](#-2-armazenamento-na-nuvem--s3-e-ebs)
3. [Criação e Uso de Imagens AMI e Snapshots EBS 🧩](#-3-criação-e-uso-de-imagens-ami-e-snapshots-ebs)
4. [Otimização de Recursos e Custos 💰](#-4-otimização-de-recursos-e-custos)
5. [Conclusão 🚀](#-5-conclusão)

---

## 🖥️ 1. Computação na Nuvem – Amazon EC2  

O **Amazon EC2 (Elastic Compute Cloud)** é um serviço de **computação sob demanda** que oferece **máquinas virtuais configuráveis** (instâncias).  
Essas instâncias fazem parte do modelo **IaaS (Infraestrutura como Serviço)**, e o usuário é responsável por aplicativos, dados e conexões.

Cada instância EC2 é composta por:
- 💡 **CPU, Memória, Disco, Rede e Sistema Operacional**

### 🔹 Tipos de Instâncias EC2  

| Categoria | Descrição | Exemplos (Séries) |
|------------|------------|------------------|
| **General Purpose** | Uso geral: servidores web, pequenos bancos de dados | A1, T2, M4 |
| **Compute Optimised** | Foco em alto desempenho de CPU | C4 |
| **Memory Optimised** | Ideal para aplicações que exigem muita memória (SAP, Spark, etc.) | R4, X1, z1d |
| **Accelerated Computing** | Machine Learning, gráficos e processamento pesado | P2, G3, F1 |
| **Storage Optimised** | Alto throughput de disco, Big Data e Data Warehousing | H1, I3, D2 |

---

## 🗄️ 2. Armazenamento na Nuvem – S3 e EBS  

### 🧱 Amazon S3 (Simple Storage Service)  

O **S3** é um serviço de **armazenamento de objetos** seguro, escalável e altamente durável.  
Ideal para armazenar grandes volumes de dados e acessá-los globalmente.

| Classe | Frequência de Acesso | Objetivo Principal |
|--------|---------------------|--------------------|
| **S3 Standard** | Frequente | Alta disponibilidade e performance |
| **S3 Standard-IA** | Infrequente | Menor custo, acesso imediato |
| **S3 One Zone-IA** | Infrequente | Mais econômico, porém limitado a uma AZ |
| **S3 Glacier / Deep Archive** | Raro | Armazenamento de baixo custo para arquivamento |

🔁 **Lifecycle Policies:** permitem mover objetos automaticamente entre classes, otimizando custos.

---

### 💽 Amazon EBS (Elastic Block Store)  

O **EBS** fornece **armazenamento em blocos persistente** para instâncias EC2.  
Funciona como um **disco rígido virtual** anexado à instância.

- 📦 **Expansão rápida de capacidade**  
- 🔒 **Alta confiabilidade e persistência**  
- 🧰 **Usos comuns:** bancos de dados, aplicações web e logs de sistema  

---

## 🧩 3. Criação e Uso de Imagens AMI e Snapshots EBS  

### 🖼️ Amazon Machine Image (AMI)  

A **AMI (Amazon Machine Image)** é um **modelo pré-configurado de instância EC2**, que contém:
- Sistema operacional  
- Configurações, pacotes e permissões  
- Volumes EBS associados  

📦 **Usos da AMI:**
- Criar novas instâncias EC2 rapidamente com o mesmo ambiente.  
- Padronizar servidores (ex: web servers idênticos).  
- Fazer backup de configurações importantes.

🧰 **Tipos de AMI:**
- **Public AMIs:** fornecidas pela AWS ou comunidade (ex: Ubuntu, Amazon Linux)  
- **Private AMIs:** criadas e mantidas pelo próprio usuário  
- **Marketplace AMIs:** disponibilizadas por terceiros (ex: WordPress, Jenkins)

🛠️ **Criação de uma AMI personalizada:**
1. Configure sua instância EC2.  
2. No console, selecione **Actions → Image and templates → Create image**.  
3. Dê um nome e descrição.  
4. A AWS criará uma imagem reutilizável com o estado atual da instância.  

---

### 📸 Snapshots EBS  

Um **Snapshot EBS** é uma **cópia de segurança incremental** de um volume EBS.  
Ele captura o estado do volume em um ponto no tempo.

📦 **Usos do Snapshot:**
- Backup e recuperação de dados.  
- Criação de novos volumes a partir de um backup existente.  
- Migração de dados entre regiões ou contas AWS.

🔁 **Relação entre AMIs e Snapshots:**
- Quando você cria uma AMI, a AWS **gera automaticamente um snapshot EBS** do volume raiz.  
- Esses snapshots são armazenados no **S3** e podem ser usados para **restaurar volumes** posteriormente.

---

## 💰 4. Otimização de Recursos e Custos  

Otimizar recursos significa aumentar eficiência e reduzir gastos.  
A AWS oferece diversas estratégias para isso:

| Estratégia | Descrição |
|-------------|------------|
| **Desligar instâncias não utilizadas** 🛑 | Economize em ambientes de teste e treinamento. |
| **Remover recursos ociosos** 🗑️ | Evite custos com recursos parados. |
| **Escalabilidade Vertical** ⬆️ | Aumente recursos no mesmo servidor. |
| **Escalabilidade Horizontal** ➡️ | Adicione novas instâncias conforme a demanda. |

### 🛒 Tipos de Compra de Instâncias EC2  

| Tipo | Vantagem | Recomendação |
|------|-----------|--------------|
| **Sob Demanda (On-Demand)** ⏳ | Pagamento por hora | Testes e workloads curtos |
| **Instâncias Reservadas** 💰 | Descontos até 75% | Uso contínuo e previsível |
| **Instâncias Spot** ⚡ | Desconto até 90% | Tarefas flexíveis e não críticas |

---

## 🚀 5. Conclusão  

O Módulo 2 da Formação **AWS Cloud Foundations** apresenta os conceitos essenciais de computação e armazenamento na nuvem, destacando:

- 🧠 **EC2:** infraestrutura escalável e flexível  
- 💾 **S3 e EBS:** soluções robustas e seguras para armazenamento  
- 🧩 **AMI e Snapshots:** automação, backup e padronização de servidores  
- 💸 **Otimização de recursos:** redução de custos sem perder desempenho  

⚡ **A base da nuvem AWS é compreender como escalar, otimizar e gerenciar recursos de forma inteligente e econômica.**


