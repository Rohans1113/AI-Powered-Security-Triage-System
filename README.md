# AI-Powered-Security-Triage-System

🛡️ AI-Powered Security Triage System
An intelligent automation layer designed to sit between your SIEM/EDR and your SOC analysts. This system leverages Large Language Models (LLMs) and Machine Learning to automatically categorize, enrich, and prioritize security alerts, reducing "alert fatigue" by up to 80%.

#  Overview
Modern Security Operations Centers (SOCs) are overwhelmed by thousands of low-fidelity alerts. This system acts as a Tier 1 Analyst by:
Clustering: Grouping related alerts (e.g., multiple failed logins from one IP) into a single incident.
Contextual Enrichment: Automatically pulling data from Threat Intel (VirusTotal, AlienVault) and internal asset logs.
Risk Scoring: Assigning a dynamic priority score based on business impact and threat severity.
Disposition Suggestion: Recommending whether to Escalate, Close as False Positive, or Monitor.

#  Tech Stack
Core Logic: Python 3.10+
AI/ML: LangChain, OpenAI GPT-4 / Anthropic Claude 3.5, Scikit-Learn (for local anomaly detection).
Data Ingestion: FastAPI / Webhooks (supports Splunk, Sentinel, CrowdStrike).
Database: PostgreSQL (Metadata) & Pinecone/ChromaDB (Vector store for historical alert context).
Orchestration: Docker & GitHub Actions.
