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

- [ ] **Phase 1** — Kafka streaming pipeline + 
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

