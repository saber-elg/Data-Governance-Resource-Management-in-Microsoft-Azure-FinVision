# 🏦 FinVision: Azure Data Governance & Resource Management Platform

[![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white)](https://azure.microsoft.com/)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Apache Spark](https://img.shields.io/badge/Apache%20Spark-E25A1C?style=for-the-badge&logo=apache-spark&logoColor=white)](https://spark.apache.org/)
[![Microsoft Purview](https://img.shields.io/badge/Microsoft%20Purview-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)](https://www.microsoft.com/en-us/security/business/microsoft-purview)

> A comprehensive enterprise-grade data governance and resource management solution built on Microsoft Azure, demonstrating best practices for financial data processing, security compliance, and cost optimization.

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Architecture](#-architecture)
- [Key Features](#-key-features)
- [Technology Stack](#-technology-stack)
- [Project Results](#-project-results)
- [Cost Analysis](#-cost-analysis)
- [Demo](#-demo)
- [Security & Compliance](#-security--compliance)
- [Future Enhancements](#-future-enhancements)

---

## 🎯 Overview

**FinVision** is an end-to-end data governance platform designed for financial institutions to manage, secure, and classify sensitive data while ensuring regulatory compliance and operational traceability. Built following the **Microsoft Cloud Adoption Framework (CAF)**, this project processes over **6.3 million financial transactions** with 100% security compliance and optimal cost efficiency.

### 🎓 Academic Context
- **Institution**: Data Engineering Program
- **Academic Year**: 2025/2026
- **Project Duration**: 25 days
- **Supervisor**: Mme Hayat Routaib

### 🔑 Key Objectives

1. **Technical Excellence**
   - Deploy CAF-compliant cloud infrastructure
   - Implement scalable Big Data platform
   - Automate data governance with Microsoft Purview
   - Ensure security through RBAC and Azure Policies
   - Maintain costs under $100/month

2. **Educational Goals**
   - Master Azure ecosystem services
   - Understand data governance principles
   - Strengthen Big Data and cloud security skills

---

## 🏗 Architecture

### System Architecture Overview

<img width="1400" height="900" alt="Image" src="https://github.com/user-attachments/assets/2ba2d915-3ee6-4e57-b466-440d37c74124" />



![Image](https://github.com/user-attachments/assets/577b391b-b739-4840-b832-073fc927ca70)

### Data Flow Architecture

![Image](https://github.com/user-attachments/assets/9d09f269-f629-4293-8a03-dd04c1a81f49)

---

## ✨ Key Features

### 🔐 Data Governance
- **Automated Discovery**: Microsoft Purview scans and catalogs 5+ data assets automatically
- **Intelligent Classification**: Auto-classification of 12+ sensitive columns (PII, financial data)
- **Complete Lineage**: End-to-end data lineage tracking from raw → curated → SQL
- **Centralized Catalog**: Searchable metadata repository with enriched business context

### 🚀 Big Data Processing
- **High Performance**: 6,362,620 transactions processed in 8 minutes (12,940 rows/sec)
- **Distributed Computing**: Apache Spark on Azure Synapse with auto-scaling (3-6 nodes)
- **Optimized Storage**: Parquet format achieving 60% compression ratio vs CSV
- **Fraud Detection**: Real-time identification of suspicious transactions (0.129% fraud rate)

### 🔒 Security & Compliance
- **Zero-Trust Security**: Role-Based Access Control (RBAC) on all resources
- **Policy Enforcement**: Azure Policies ensuring 100% compliance (encryption, HTTPS)
- **Data Encryption**: At-rest and in-transit encryption with Microsoft-managed keys
- **Audit Trail**: Complete logging and monitoring of all data access

### 💰 Cost Optimization
- **Budget Management**: Actual cost $30/month vs $100 budget (70% savings)
- **Auto-Scaling**: Dynamic resource allocation based on workload
- **Smart Storage**: LRS replication + lifecycle management + compression
- **Auto-Pause**: 15-minute idle timeout on Spark pools

---

## 🛠 Technology Stack

### Cloud Platform
| Service | Purpose | Configuration |
|---------|---------|---------------|
| **Azure Data Lake Storage Gen2** | Hierarchical data lake | Standard_LRS, 500GB |
| **Azure SQL Database** | Relational database | Basic tier, 5 DTU |
| **Azure Synapse Analytics** | Big Data analytics | Serverless + Spark Pool |
| **Microsoft Purview** | Data governance | Single collection |
| **Azure Policy** | Compliance enforcement | 2 active policies |

### Development Tools
- **Language**: Python 3.x, PySpark
- **Notebook Environment**: Synapse Studio
- **Data Format**: CSV (raw), Parquet (curated)
- **Authentication**: Managed Identity, RBAC

### Data Processing
```python
# Core Technologies
- Apache Spark 3.3
- PySpark DataFrames API
- Delta Lake format
- SQL Server T-SQL
```

---

## 📊 Project Results

### Performance Metrics

| Metric | Value | Target | Status |
|--------|-------|--------|--------|
| **Processing Time** | 8m 12s | < 10 min | ✅ |
| **Rows Processed** | 6,362,620 | 6M+ | ✅ |
| **Throughput** | 12,940 rows/sec | > 10K | ✅ |
| **Data Completeness** | 99.98% | > 99% | ✅ |
| **Security Compliance** | 100% | 100% | ✅ |
| **Monthly Cost** | $30 | < $100 | ✅ |

### Storage Optimization

| Format | Size | Compression | Read Time |
|--------|------|-------------|-----------|
| CSV (raw) | 498 MB | 0% | 45 sec |
| Parquet (curated) | 187 MB | 62.5% | 4 sec |

### Transaction Analysis

| Transaction Type | Volume | Fraud Cases | Fraud Rate |
|-----------------|--------|-------------|------------|
| TRANSFER | 532,909 | 4,097 | 0.769% |
| CASH_OUT | 2,237,500 | 4,116 | 0.184% |
| PAYMENT | 2,151,495 | 0 | 0.000% |
| CASH_IN | 1,399,284 | 0 | 0.000% |
| DEBIT | 41,432 | 0 | 0.000% |
| **TOTAL** | **6,362,620** | **8,213** | **0.129%** |

---


## 💵 Cost Analysis

### Cost Management Dashboard
![Image](https://github.com/user-attachments/assets/b6a4c661-e03e-4545-be94-54ae1826d645)

</details>

### Cost Optimization Strategies

1. **Storage Tier**: LRS instead of GRS (-50%)
2. **SQL Database**: Basic tier instead of Standard (-70%)
3. **Spark Pool**: Auto-pause after 15 minutes of inactivity
4. **Auto-Scaling**: Dynamic allocation (3-6 nodes vs fixed 6)
5. **Compression**: Parquet format reduces storage by 60%
6. **Purview Scans**: Manual/on-demand instead of scheduled weekly


---

## 🎥 Demo

### Video Demonstration
\
**📺 [Watch Full Demo Video](https://www.youtube.com/watch?v=YOUR_VIDEO_ID)** *(25 minutes)*

**Demo Highlights:**
- ✅ Live infrastructure walkthrough
- ✅ PySpark notebook execution (6.3M transactions)
- ✅ Purview data discovery and classification
- ✅ Data lineage visualization
- ✅ Security compliance validation
- ✅ Cost dashboard review

---

## 🔐 Security & Compliance

### Security Implementation

#### 1. Identity & Access Management
```yaml
RBAC Assignments:
  - Storage Blob Data Contributor: Synapse Managed Identity
  - SQL Server Contributor: Data Engineers
  - Purview Data Curator: Governance Team
  - Reader: Auditors
```

#### 2. Network Security
- **Private Endpoints**: Enabled for SQL Database
- **Firewall Rules**: Whitelist Azure services only
- **Public Access**: Disabled on storage accounts
- **TLS**: Minimum version 1.2 enforced

#### 3. Data Protection
- **Encryption at Rest**: Microsoft-managed keys
- **Encryption in Transit**: HTTPS/TLS 1.2+
- **Backup**: 7-day retention for SQL Database
- **Soft Delete**: 14-day recovery window

#### 4. Compliance Policies

| Policy | Status | Resources Affected |
|--------|--------|-------------------|
| Enforce HTTPS | ✅ Active | All storage accounts |
| Require encryption | ✅ Active | All data services |
| Mandatory tagging | ✅ Active | All resources |
| Location restriction | ✅ Active | France Central only |

### GDPR Compliance

- ✅ **Right to Access**: Data catalog in Purview
- ✅ **Right to Erasure**: Soft delete enabled
- ✅ **Data Minimization**: Only essential fields stored
- ✅ **Purpose Limitation**: Clear data usage policies
- ✅ **Audit Trail**: Complete activity logging

---

## 🔮 Future Enhancements

### Short-term 

#### Analytics & BI
- [ ] Power BI dashboards (Fraud Analytics, Transactions, Clients)
- [ ] Real-time monitoring with Power BI streaming
- [ ] Custom KPI development

#### CI/CD Pipeline
- [ ] Azure DevOps integration
- [ ] Automated notebook testing
- [ ] Branch strategy (main/dev/feature)
- [ ] Automated deployment to production

#### Advanced Alerting
- [ ] Azure Monitor alerts for job failures
- [ ] Logic Apps for fraud notification (>$1000)
- [ ] ServiceNow integration for incidents


---

## 📞 Contact

For questions or collaboration opportunities:

- 📧 Email: medsaberelguelta@gmail.com  
- 💼 LinkedIn: [Your LinkedIn](https://linkedin.com/in/mohamed-saber-elguelta)
- 🐙 GitHub: [@saber-elg](https://github.com/saber-elg)

---

