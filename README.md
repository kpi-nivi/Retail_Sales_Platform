# Retail_Sales_Platform
Building end-to-end retail analytics pipeline | AI-powered  |  Kafka → Snowflake → Databricks → DBT → Tableau |  LLM-integrated data quality, insights &amp; NL-to-SQL

# 🛒 AI-Powered Retail Sales Intelligence Platform

An end-to-end data engineering portfolio project simulating 
a production-grade retail analytics pipeline with AI/LLM 
integration at every layer of the stack.

---

## 🏗️ Architecture
```
Kafka Producer → Kafka Consumer → Snowflake Bronze
→ AI Quality Checker (Claude API)
→ Azure Databricks PySpark → Snowflake Silver
→ DBT Models → Snowflake Gold
→ Tableau Dashboard
→ NL-to-SQL Chatbot (Streamlit)
```

---

## 🤖 AI Integration

| Layer | AI Feature |
|---|---|
| Data Quality | Anomaly detection with plain-English explanations |
| Transformation | Business insights after every pipeline run |
| Dashboard | Auto-generated weekly CEO narrative |
| Chatbot | Natural language to SQL conversion |
| Alerting | Smart root cause analysis on failures |

---

## 🛠️ Tech Stack

| Layer | Tools |
|---|---|
| Ingestion | Apache Kafka, Python |
| Storage | Snowflake (Bronze/Silver/Gold) |
| Processing | PySpark, Azure Databricks |
| Modeling | DBT |
| Visualization | Tableau |
| AI/LLM | Claude API (Anthropic) |
| App | Streamlit |
| CI/CD | GitHub Actions |
| Scripting | Python, Shell |

---

## 📁 Project Structure
```
retail-intelligence-platform/
├── ingestion/
│   ├── producer.py          # Kafka producer
│   ├── consumer.py          # Kafka consumer → Snowflake
│   └── config.py            # Connection config
├── quality/
│   ├── checks.py            # Data quality checks
│   ├── ai_explainer.py      # Claude API anomaly explainer
│   └── run_pipeline.py      # Orchestrator
├── databricks/
│   └── phase2_silver.py     # PySpark transformations
├── dbt/
│   ├── models/              # Gold layer models
│   └── tests/               # Automated data tests
├── streamlit/
│   └── nl_to_sql.py         # NL-to-SQL chatbot
├── docker-compose.yml       # Kafka local setup
├── requirements.txt         # Python dependencies
└── README.md
```

---

## 🚀 Phases

- [x] **Phase 1** — Kafka streaming pipeline + 
                     Snowflake Bronze layer + 
                     AI quality checker
- [ ] **Phase 2** — PySpark Silver transformations + 
                     AI insights on Databricks
- [ ] **Phase 3** — DBT Gold models + 
                     automated testing + CI/CD
- [ ] **Phase 4** — Tableau executive dashboard
- [ ] **Phase 5** — NL-to-SQL Streamlit chatbot
- [ ] **Phase 6** — Smart alerting + monitoring

---

## ⚙️ Setup

### Prerequisites
```bash
Python 3.11+
Docker Desktop
Snowflake account (free trial)
Azure Databricks account
Anthropic API key
```

### Installation
```bash
# Clone the repo
git clone https://github.com/yourusername/retail-intelligence-platform.git

# Create virtual environment
python3.11 -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Fill in your credentials in .env
```

### Run Phase 1
```bash
# Start Kafka
docker compose up -d

# Terminal 1 — Start consumer
python ingestion/consumer.py

# Terminal 2 — Stream transactions
python ingestion/producer.py

# Run AI quality checks
python quality/run_pipeline.py
```

---

## 📊 Sample Output

### AI Quality Check Report
```
✅ PASSED | null_region_check    | Value: 0
❌ FAILED | revenue_spike_check  | Value: 3
🤖 AI Explanation: Three transactions show 
   unusually high revenue exceeding $50K, 
   suggesting data entry errors at the POS 
   system. Recommend validating input controls 
   at source systems.
```

### PySpark Transformation Summary
```
✅ Records loaded   : 200
✅ Records cleaned  : 187
🗑️  Records removed  : 13
🤖 AI Insight: The 6.5% data removal rate 
   indicates moderate quality issues upstream...
```

---

## 🎥 Demo
[Loom video walkthrough] ← Add your link here

---

## 👩‍💻 Author
**Nivitha Sambath Kumar**
Lead Data Analyst | Data Engineer
[LinkedIn](https://linkedin.com/in/yourprofile) | 
[GitHub](https://github.com/yourusername)
```

---

## Topics to Add to GitHub Repo

When creating the repo, add these topics — they make your repo discoverable:
```
apache-kafka
snowflake
pyspark
azure-databricks
dbt
tableau
streamlit
anthropic
llm
data-engineering
medallion-architecture
portfolio-project
python
etl-pipeline
```

---

## How to Add Topics
```
Your GitHub repo page
→ Click ⚙️ gear icon next to "About"
→ Add topics one by one
→ Save changes
```

---

## Create requirements.txt

Add this file to your project root so anyone can install dependencies:
```
confluent-kafka==2.3.0
snowflake-connector-python==3.6.0
pandas==2.1.0
faker==19.6.0
anthropic==0.84.0
python-dotenv==1.0.0
pyspark==3.4.1
streamlit==1.28.0
dbt-snowflake==1.6.0
```

---

## Create .env.example

Add this file so others know what credentials are needed without exposing yours:
```
SNOWFLAKE_USER=your_username
SNOWFLAKE_PASSWORD=your_password
SNOWFLAKE_ACCOUNT=your_account
SNOWFLAKE_DATABASE=RETAIL_DB
SNOWFLAKE_SCHEMA=BRONZE
SNOWFLAKE_WAREHOUSE=COMPUTE_WH
KAFKA_BROKER=localhost:9092
ANTHROPIC_API_KEY=your_api_key
