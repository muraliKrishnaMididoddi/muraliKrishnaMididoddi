<h1 align="left">Hi, I'm Murali 👋</h1>

**Data Engineer.** I build pipelines that real teams depend on: healthcare claims, regulatory reporting, CRM, and LLM-powered workflows in production.

<p align="left">
  <a href="https://muralikrishnamididoddi.github.io/Murali_portfolio.github.io/"><img src="https://img.shields.io/badge/Portfolio-27CBCB?style=flat-square&logo=googlechrome&logoColor=0e1116" alt="Portfolio"/></a>
  <a href="https://www.linkedin.com/in/murali-data-engineer-scientist"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:munnummk499@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"/></a>
  <img src="https://img.shields.io/badge/status-open%20to%20work-26D868?style=flat-square" alt="Open to work"/>
</p>

My own measure of my work is simple: **if nobody depends on it, it isn't shipped yet.** That's why this profile starts with the systems people use, not my commit graph.

---

## 🚀 Shipped: systems with real users

| What I built | Who uses it | What changed |
|---|---|---|
| **Guest-feedback triage** (Delaware North / TD Garden). An LLM pipeline (LangChain, Hugging Face, RAG) that classifies guest survey comments and routes actionable issues into Salesforce. | Guest experience & operations teams | Feedback becomes a Salesforce case for the team that can fix it |
| **Incremental Databricks → Redshift sync** (Delaware North). Delta Sharing + Change Data Feed, orchestrated with Step Functions and Lambda, with Glue API integrations, retries, and CloudWatch alerting. | Analytics, reporting & ML consumers | Incremental loads instead of full reloads |
| **HIPAA claims data platform** (Aetna, CVS Health). S3 data lake, Glue ETL, and partitioned Athena/Redshift layers, with Jenkins CI/CD. | Clinical, operational & finance reporting teams (self-service) | **30% faster queries** on 5M+ record batches; **zero audit findings over 22 months** |
| **Regulatory reporting automation** (Prasquare Technologies). Automated ETL, validation, and reconciliation for FHFA and risk reporting, with audit-ready lineage. | Risk, Finance & Data Management teams | **~12 hrs/week** of manual prep eliminated; **30%** better reporting visibility |
| **CRM migration & ledger reconciliation** (Rollins, Inc.). Cleansing, mapping, and source-to-target validation, plus ERP/CRM/ledger integration via ADF and Synapse. | Finance & operations stakeholders | **100K+ records migrated with zero data loss** |

Across these roles, reconciliation and data-quality controls prevented roughly **$5.2M in reporting errors**.

---

## 🔓 Open source

**[LLM Rate-Limit Backpressure Engine](https://github.com/muraliKrishnaMididoddi/llm-backpressure-engine)**: queues and paces requests when many services share one LLM API quota, so 429s don't cascade.
Per-tenant Redis token buckets (atomic Lua) · Kafka priority lanes · backoff with jitter · Grafana dashboards · one `docker compose up`.

**[Distributed Document Ingestion + RAG](https://github.com/muraliKrishnaMididoddi/rag-pipeline)**: retrieval over legal, pharma, and technical PDFs, with evaluation built in. Started as my MS capstone and hardened since.
Docling → chunking → PII redaction → Bedrock embeddings → Pinecone + Neo4j · ECS Fargate workers on SQS · hybrid retrieval + reranking · Precision@k / Recall@k / RAG-triad evals.

Issues, forks, and "this breaks when…" reports are welcome.

---

## 📝 Notes from production

Things real pipelines taught me. I write about them [on LinkedIn](https://www.linkedin.com/in/murali-data-engineer-scientist/recent-activity/all/).

- **The code is rarely the problem; the CSV is.** A file had 12 columns yesterday and 13 today. Schema checks at ingestion beat a 2 a.m. failure.
- **Cloud migration is never just lift and shift.** SFTP, IP allowlisting, failure handling, and what happens when the same file arrives twice.
- **"It was working yesterday."** Hours of debugging traced back to an expired credential. Secrets rotation is part of the pipeline.
- **Undocumented pipelines are a liability.** The day the author leaves, "does anyone know how this works?" becomes a crisis.

---

## 🧰 Stack

`Python` `SQL` `PySpark` `Databricks` `Delta Lake` `Snowflake` `dbt` `Kafka` `Airflow`
`AWS: Glue · Lambda · Step Functions · Redshift · Athena · EMR · SageMaker · Bedrock`
`Azure: Data Factory · Synapse · ADLS Gen2` `LangChain` `Hugging Face` `Pinecone` `Neo4j`
`Docker` `Kubernetes` `Terraform` `Jenkins` `Salesforce` `MuleSoft` `Power BI`

---

## 💼 Experience

| Role | Company | When |
|---|---|---|
| Data Engineer | Delaware North (TD Garden) · Remote | Jul 2026 – Present |
| Analyst, CRM Analytics | Delaware North (TD Garden) | May – Jul 2026 |
| Data Specialist (Contract) | Rollins, Inc. · Atlanta | Aug 2025 – Mar 2026 |
| Data Analyst, Mortgage Analytics (Contract) | Prasquare Technologies · Remote | Feb – Aug 2025 |
| Data Engineer (Contract) | Aetna, a CVS Health Company · Remote | Jan 2021 – Dec 2022 |
| Senior Analyst, FP&A | Aetna, a CVS Health Company | Jan – Dec 2020 |

**Education:** MS Big Data Analytics, University of Central Missouri (GPA 3.70) · B.Tech, KKR & KSR Institute of Technology & Sciences
**Certifications:** AWS ML Specialty · Databricks Certified Data Engineer · Microsoft PL-300 · AWS Cloud Practitioner · Databricks GenAI Fundamentals · DeepLearning.AI Agentic AI

---

## 📫 Let's talk

I'm open to **Data Engineering and ML Data Engineering** roles: full-time or contract, in Atlanta or Boston, or remote.
If your team has data it can't trust yet, I'd like to hear about it.

**Email:** [munnummk499@gmail.com](mailto:munnummk499@gmail.com) · **LinkedIn:** [in/murali-data-engineer-scientist](https://www.linkedin.com/in/murali-data-engineer-scientist) · **Portfolio:** [muralikrishnamididoddi.github.io](https://muralikrishnamididoddi.github.io/Murali_portfolio.github.io/)

<sub>Older ML/analytics learning notebooks live in [PortfolioProjects](https://github.com/muraliKrishnaMididoddi/PortfolioProjects).</sub>


<!----

## About Me

Hello! I'm **Murali Krishna Mididoddi**, a **Senior Data Engineer** with 5+ years of experience building **HIPAA-compliant data platforms**, **enterprise-scale pipelines**, and **production AI/ML infrastructure** across healthcare, financial services, and sports & entertainment.

I specialize in turning regulated, high-volume data into reliable, scalable systems that can withstand production demands, audits, and evolving business requirements.

**Career highlights**
- **Aetna (CVS Health):** architected HIPAA-compliant AWS data infrastructure processing 5M+ healthcare claim records, cut query latency by 30%, and supported **22 months with zero audit findings**
- **Federal Home Loan Bank of Atlanta:** automated FHFA regulatory reporting workflows, eliminating ~**12 hours/week** of manual data preparation with audit-ready lineage and traceability
- **Rollins, Inc.:** designed enterprise lakehouse architecture (Azure Data Factory, ADLS Gen2, Databricks, Bronze-Silver-Gold) supporting operations, financial analytics, and ML workloads
- **GenAI / AI Engineering:** a Distributed RAG Pipeline (Pinecone, Neo4j, ECS Fargate, Amazon Bedrock) and an LLM Rate-Limit Backpressure Engine (Kafka, Redis, FastAPI) addressing millions of monthly API failures

```python
murali = {
    "role":        "Senior Data Engineer",
    "location":    "Atlanta Metropolitan Area (open to NYC, Boston + 3 more)",
    "open_to":     ["Senior Data Engineer", "Healthcare Data Engineer", "AI Engineer",
                    "Generative AI", "Machine Learning Engineer", "Data Platform Engineer"],
    "experience":  "5+ years",
    "education":   "MS Big Data Analytics — University of Central Missouri (GPA 3.70)",
    "certifications": ["AWS ML Specialty", "AWS Cloud Practitioner"],
    "top_skills":  ["Docker / Kubernetes", "Terraform", "dbt", "LangChain", "AWS SageMaker"],
    "focus":       ["Data Platforms", "Lakehouse Architecture", "RAG & LLM Infrastructure",
                    "Governance & Compliance (HIPAA / SOX / FINRA)"],
    "contact":     "munnummk499@gmail.com"
}
```

## Recruiter Snapshot

- 5+ years in data engineering across healthcare, financial services, and sports & entertainment
- HIPAA-compliant and audit-ready pipelines zero audit findings over 22 months at Aetna
- Core stack: Python, SQL, PySpark, Databricks, Snowflake, AWS Glue, Lambda, Redshift, Athena, Azure Data Factory, Kafka, Terraform, dbt, FastAPI, LangChain, Hugging Face, Pinecone, Neo4j, Salesforce CRM, MuleSoft
- AI/ML:RAG, vector databases, model evaluation, retrieval quality analysis, agent orchestration, and AI-assisted development tools (Claude Code, Cursor, Codex)
- AWS Certified Machine Learning Specialty| AWS Cloud Practitioner
- Comfortable across the full lifecycle: ingestion, transformation, orchestration, storage, data quality, lineage, governance, APIs, model integration, evaluation, observability, and production deployment
- Currently open to work — full-time, W2 contract, remote, hybrid, and on-site

---

## Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,azure,aws,docker,kubernetes,terraform,github,postgresql,java,tensorflow,pytorch,kafka,redis,bash,linux&perline=5" />
</p>

<br/>

### 🤖 AI & Machine Learning
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![SageMaker](https://img.shields.io/badge/AWS%20SageMaker-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-000000?style=flat-square)
![Neo4j](https://img.shields.io/badge/Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=white)

### 🚦 LLM Infrastructure
![Kafka](https://img.shields.io/badge/Apache%20Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Amazon Bedrock](https://img.shields.io/badge/Amazon%20Bedrock-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)

### 📊 Data Engineering
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-56B9EB?style=flat-square&logo=snowflake&logoColor=white)
![Delta Lake](https://img.shields.io/badge/Delta%20Lake-003366?style=flat-square)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)

### ☁️ Cloud Platforms
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![AWS Glue](https://img.shields.io/badge/AWS%20Glue-232F3E?style=flat-square)
![Athena](https://img.shields.io/badge/AWS%20Athena-232F3E?style=flat-square)
![Redshift](https://img.shields.io/badge/Amazon%20Redshift-8C4FFF?style=flat-square)
![Lambda](https://img.shields.io/badge/AWS%20Lambda-FF9900?style=flat-square&logo=awslambda&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![ADF](https://img.shields.io/badge/Azure%20Data%20Factory-0078D4?style=flat-square)
![ADLS Gen2](https://img.shields.io/badge/ADLS%20Gen2-0078D4?style=flat-square)

### 💻 Languages
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)

### 🔧 Orchestration & DevOps
![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=flat-square&logo=terraform&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)

### 🧩 CRM & Integration
![Salesforce](https://img.shields.io/badge/Salesforce-00A1E0?style=flat-square&logo=salesforce&logoColor=white)
![MuleSoft](https://img.shields.io/badge/MuleSoft-00A0DF?style=flat-square&logo=mulesoft&logoColor=white)

---

## Core Competencies

- **Data Platform Engineering** — ETL/ELT, batch & incremental processing, orchestration, CI/CD
- **Lakehouse Architecture** — Azure Data Factory, ADLS Gen2, Databricks, Bronze-Silver-Gold
- **Regulated Data & Governance** — HIPAA, SOX, FINRA, FHFA reporting, lineage, auditability
- **GenAI / AI Engineering** — RAG, LLM infrastructure, vector databases, agent orchestration, evaluation
- **Machine Learning & MLOps** — feature pipelines, model comparison, deployment, monitoring
- **Cloud Data Services** — AWS and Azure at scale
- **Data Quality & Observability** — validation frameworks, idempotency, retries, failure handling
- **CRM & Operational Data Integration** — Salesforce CRM, MuleSoft

---

## Experience

### Delaware North (TD Garden) — Remote

**Associate Data and AI Engineer** (Jul 2026 – Present · 3 mos)
- Building a survey analysis-to-insights MLOps pipeline using Python and ETL workflows

**Senior Analyst | CRM Analytics** (May 2026 – Jul 2026 · 3 mos)
- Managed Salesforce CRM workflows, user access, and MuleSoft integrations to support secure CRM operations
- Developed ETL pipelines using SQL, Python, PostgreSQL, Redshift, and Databricks to improve data quality
- Delivered Power BI, Tableau, and Salesforce dashboards for CRM, KPI, and operational reporting
- Led Salesforce migration validation by cleansing and reconciling records across internal and external systems

---

### ML Engineer, Azure & AWS Data Platform | Rollins, Inc. — Atlanta, GA (Contract, Aug 2025 – Mar 2026 · 8 mos)

- Designed enterprise lakehouse architecture (Azure Data Factory, ADLS Gen2, Databricks, Bronze-Silver-Gold) supporting operations, financial analytics, and ML workloads
- Engineered PySpark ETL pipelines processing millions of operational and financial records per batch, tuning partitioning and caching for performance
- Built reusable ingestion frameworks for structured and semi-structured sources using AWS Glue, S3, Python, and SQL
- Implemented automated data quality validation and failure-handling controls to raise reliability of financial reporting pipelines

---

### Associate Data Engineer | Federal Home Loan Bank of Atlanta — Atlanta, GA (Contract, Feb 2025 – Aug 2025 · 7 mos)

- Led data processing and integration workflows supporting financial operations, risk analytics, and FHFA regulatory reporting in a high-compliance environment
- Automated financial data preparation workflows, eliminating ~12 hours/week of manual effort with end-to-end audit-ready lineage
- Implemented role-based access, validation, and traceable change controls supporting auditability — the same rigor healthcare compliance demands

---

### Data Engineer | Aetna, a CVS Health Company — Remote (Contract, Jan 2021 – Dec 2022 · 2 yrs)

- Architected AWS-based data pipelines for healthcare claims ingestion, transformation, and regulatory reporting across high-volume datasets
- Built an Amazon S3 data lake and AWS Glue ETL workflows processing millions of healthcare records through scalable batch pipelines
- Optimized SQL transformation layers in Athena and Redshift using partitioning, cutting query latency 30% across 5M+ record batches
- Enforced healthcare data security, governance, and validation standards — zero audit findings over 22 months
- Automated CI/CD with Jenkins and GitHub, reducing manual release effort and deployment risk
- Enabled self-service analytics for clinical, operational, and finance reporting teams via curated Athena datasets

---

### Senior Analyst, FP&A – Commercial Revenue | Aetna, a CVS Health Company (Jan 2020 – Dec 2020 · 1 yr)

---

## Recent Activity
<!----
<!--RECENT_ACTIVITY:start-->
1. ⭐ Starred [oracle-devrel/oracle-ai-developer-hub](https://github.com/oracle-devrel/oracle-ai-developer-hub)
2. 🔱 Forked [muraliKrishnaMididoddi/ebook](https://github.com/muraliKrishnaMididoddi/ebook) from [learning-zone/ebook](https://github.com/learning-zone/ebook)
<!--RECENT_ACTIVITY:end-->

<!-------

## Activity Graph

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=muraliKrishnaMididoddi&theme=react-dark&hide_border=true&color=1a6b6b&line=1a6b6b&point=ffffff" />
</p>

---

## Contribution Snake

<p align="center">
  <img src="https://raw.githubusercontent.com/muraliKrishnaMididoddi/muraliKrishnaMididoddi/output/github-contribution-grid-snake-dark.svg" alt="snake animation" />
</p>

---

## LeetCode Stats

<p align="center">
  <a href="https://leetcode.com/u/MUNNUMMK499/">
    <img src="https://img.shields.io/badge/LeetCode-MUNNUMMK499-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" />
  </a>
</p>

<p align="center">
  <img src="https://leetcard.jacoblin.cool/MUNNUMMK499?theme=dark&font=Fira%20Code&ext=heatmap&border=0&radius=8" alt="LeetCode Stats" />
</p>

---

## GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=muraliKrishnaMididoddi&show_icons=true&hide_border=true&bg_color=030412&title_color=33c2cc&icon_color=7a57db&text_color=ffffff" alt="Murali GitHub stats" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=muraliKrishnaMididoddi&layout=compact&hide_border=true&bg_color=030412&title_color=33c2cc&text_color=ffffff" alt="Top Languages" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=muraliKrishnaMididoddi&theme=dark&hide_border=true&background=0D1117&ring=1a6b6b&fire=1a6b6b&currStreakLabel=1a6b6b&sideLabels=1a6b6b&dates=ffffff" alt="GitHub Streak" />
</p>

---

## Projects

### [00 · 🚦 LLM Rate-Limit Backpressure Engine](https://github.com/muraliKrishnaMididoddi/llm-backpressure-engine) ⭐ Featured Open Source
- **Solved the 8.4M monthly LLM rate-limit failure problem** with a production-grade Kafka-based backpressure engine
- Per-tenant Redis token bucket, priority queuing, exponential backoff, Grafana dashboards — full stack in one Docker command
- **Tech:** Kafka · Python · Redis · FastAPI · Prometheus · Grafana · Docker

### [01 · Distributed Document Ingestion + RAG Pipeline](https://github.com/muraliKrishnaMididoddi/rag-pipeline)
- **Production RAG for legal, pharma & technical docs** — originated as my MS capstone (Distributed RAG Pipeline for Healthcare Document Retrieval), built to production standards
- Docling layout detection → semantic chunking → PII redaction → entity extraction → Bedrock embeddings → Pinecone + Neo4j
- Distributed async workers on ECS Fargate processing thousands of PDFs concurrently with DynamoDB state tracking
- Hybrid retrieval (vector + BM25 + graph) with cross-encoder reranking; evaluated with Precision@k / Recall@k / RAG Triad
- **Tech:** Docling · Pinecone · Neo4j · ECS Fargate · DynamoDB · S3 · Bedrock · LangSmith · FastAPI

### [02 · Patient Re-admission Predictive Analytics](https://github.com/muraliKrishnaMididoddi/PortfolioProjects/blob/main/Patient%20re-admission_Predictive_Analytics.ipynb)
- Predicted patient readmissions using ML — achieved **20% reduction** in readmission rates
- Applied data preprocessing, feature engineering, and predictive modeling on clinical datasets
- **Tech:** Python, Scikit-Learn, Pandas, Healthcare Analytics

### [03 · Landing Page Optimization via A/B Testing](https://github.com/muraliKrishnaMididoddi/PortfolioProjects/blob/main/ABTesting.ipynb)
- **15% increase in conversion rates** and **10% reduction in bounce rates** through data-driven testing
- Built statistical hypothesis testing framework for digital marketing optimization
- **Tech:** Python, Scipy, Seaborn, NumPy, Statistical Analysis

### [04 · Twitter Sentiment Analysis](https://github.com/muraliKrishnaMididoddi/PortfolioProjects/blob/main/Twitter%20Sentiment%20Analysis.ipynb)
- Processed **500K+ tweets** with **98% efficiency** using NLP and transformer models
- Reduced analysis time by **40%** enabling real-time sentiment tracking
- **Tech:** Python, NLP, Transformers, Pandas

### [05 · Movie Recommendation System](https://github.com/muraliKrishnaMididoddi/PortfolioProjects/blob/main/Movie%20Portfolio%20Project.ipynb)
- **95% accuracy** in movie recommendations using collaborative filtering
- **70% improved search speed** with optimized database queries
- **Tech:** Python, Scikit-Learn, Matplotlib, NumPy, Pandas

### [06 · Clustering Wine Dataset — K-Means & DBSCAN](https://github.com/muraliKrishnaMididoddi/PortfolioProjects/blob/main/Clustering%20wine%20dataset%20with%20k-means%20and%20DBSCAN.ipynb)
- Classified **1,000+ wine samples** achieving **15% higher cluster accuracy**
- Used K-Means for segmentation and DBSCAN for outlier detection
- **Tech:** Python, K-Means, DBSCAN, Matplotlib

### [07 · SQL Data Cleaning](https://github.com/muraliKrishnaMididoddi/PortfolioProjects/blob/main/SQL%20DATA%20CLEANING.sql)
- **Reduced data duplication by 30%** through structured SQL cleaning processes
- Standardized raw datasets for enhanced integrity and downstream usability
- **Tech:** SQL, Data Quality, ETL

### [08 · House Pricing — KNN & XGBoost](https://github.com/muraliKrishnaMididoddi/PortfolioProjects/blob/main/House%20Pricing%20with%20KNN%20and%20XGBoost.ipynb)
- **15% accuracy improvement** analyzing **50K+ rows** of housing data
- Pipeline handles **1M+ rows** with **30% reduced runtime**
- **Tech:** Python, KNN, XGBoost, Feature Engineering

### [09 · Tableau Sales Analysis](https://github.com/muraliKrishnaMididoddi/PortfolioProjects/blob/main/tableau%20analysis%201.twbx)
- Interactive dashboards identifying sales trends — resulted in **10% revenue increase**
- **Tech:** Tableau, BI, Sales Analytics

### [10 · Student Management System](https://github.com/muraliKrishnaMididoddi/studentmngt)
- Full-stack Spring Boot app — **25% improved data accuracy**, **40% reduced processing time**
- **Tech:** Java, Spring Boot, HTML, SQL

### [11 · Credit Card Fraud Detection](https://github.com/muraliKrishnaMididoddi/PortfolioProjects/blob/main/Credit%20Card%20Fraud%20Detection%20-%20Decision%20Tree.ipynb)
- **99.3% accuracy** on 284K transactions using Decision Tree + SMOTE
- **30% reduced fraud detection latency** enabling real-time screening
- **Tech:** Python, Decision Tree, SMOTE, Pandas

### [12 · Collaborative Filtering Recommendation Engine](https://github.com/muraliKrishnaMididoddi/collaborative-filtering-recommendation-engine)
- ALS-based Spark MLlib engine processing **2M+ user-item interactions**
- Generated **top-10 recommendations for 2M+ users** with **0.87 RMSE**
- **Tech:** PySpark, Apache Spark, MLlib, ALS, Collaborative Filtering

---

## Education

### Master's Degree, Big Data Analytics
**University of Central Missouri** — Warrensburg, United States
Jan 2023 – Dec 2024 | **GPA: 3.70**
Relevant coursework: Big Data Analytics · Data Mining · Statistical Methods · Machine Learning · Database Management · Business Intelligence · Information Visualization · Project Management · Natural Language Processing
Capstone: Distributed RAG Pipeline for Healthcare Document Retrieval — built an end-to-end RAG system using Pinecone, Neo4j, and AWS Bedrock, demonstrating production-grade AI engineering beyond coursework

### Bachelor's Degree
**KKR&KSR Institute of Technology & Sciences** — Vinjanampadu Village, India | Jul 2018 – Jul 2022

---

## Certifications

| Certification | Valid |
|---|---|
| 🏆 AWS Certified Machine Learning: Specialty | Feb 2025 – Feb 2028 |
| ☁️ AWS Certified Cloud Practitioner | Sep 2024 – Sep 2027 |
| 🗄️ HackerRank SQL Certificate | Jul 2024 |
| 📐 Google: Foundations — Data, Data, Everywhere | May 2024 |
| 📐 Google: Ask Questions to Make Data-Driven Decisions | May 2024 |
| 📐 Google: Prepare Data for Exploration | Jun 2024 |
| 🌐 VMware IT Academy Network Virtualization | Jan 2021 |

---

## Publications

**A Statistical Survey of Energy Efficient WSN Protocols in Communication Networks — Part 1**, MAT Journals

---

## Open to Opportunities

I'm actively exploring roles in:

- 🔹 Senior Data Engineer
- 🔹 Healthcare Data Engineer
- 🔹 AI Engineer / Generative AI
- 🔹 Machine Learning Engineer
- 🔹 Data Platform Engineer

Especially interested in roles where **reliability, governance, security, and regulatory rigor** are core engineering requirements — full-time, W2 contract, remote, hybrid, or on-site, based in the Atlanta metro area or the NYC/Boston metro areas.

If your team is hiring, or you know someone who is, I'd appreciate a connection or referral.

---

## Contact

| | |
|---|---|
| 📧 **Email** | [munnummk499@gmail.com](mailto:munnummk499@gmail.com) |
| 📞 **Phone** | (470) 722-4770 |
| 💼 **LinkedIn** | [linkedin.com/in/murali-krishna-data-scientist](https://www.linkedin.com/in/murali-krishna-data-scientist/) |
| 🐙 **GitHub** | [github.com/muraliKrishnaMididoddi](https://github.com/muraliKrishnaMididoddi) |
| 🟡 **LeetCode** | [leetcode.com/u/MUNNUMMK499](https://leetcode.com/u/MUNNUMMK499/) |
| 🌐 **Portfolio** | [muralikrishnamididoddi.github.io/Murali_portfolio.github.io](https://muralikrishnamididoddi.github.io/Murali_portfolio.github.io/) |

---

<div align="center">
  <sub>⭐ Thank you for visiting! Open to Senior Data Engineering, AI/ML, and Data Platform roles.</sub>
</div>
```
--!>
