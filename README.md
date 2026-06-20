# LangGraph Competitive Footfall Insights

## Overview

Businesses operating in highly competitive retail locations need timely insights into nearby competitors, customer traffic patterns, and peak business hours.

This project implements a Multi-Agent AI System using LangGraph and LangChain that helps users identify nearby clothing store competitors, analyze footfall trends, evaluate peak customer hours, and generate actionable business intelligence reports.

The system combines Large Language Models (LLMs), web search capabilities, geospatial analysis, and agent-based orchestration to provide competitive market insights.

---

## Problem Statement

Businesses in competitive retail locations often struggle to monitor market rivals and understand customer traffic dynamics.

Clothing stores located in busy commercial areas face intense competition and require:

- Visibility into nearby competitors
- Footfall trend analysis
- Peak operating hours
- Competitive benchmarking
- Location-based market intelligence

This project addresses these challenges through an AI-powered conversational analytics pipeline.

---

## Intended Beneficiaries

### Business Owners & Store Managers

- Identify nearby competitors
- Understand market saturation
- Analyze customer traffic patterns
- Improve operational planning

### Marketing & Strategy Teams

- Optimize promotions during high-traffic periods
- Benchmark competitor activity
- Improve local engagement campaigns

### Real Estate & Location Analysts

- Evaluate potential store locations
- Assess location attractiveness
- Support expansion planning

### Investors & Market Analysts

- Analyze retail market opportunities
- Assess competition density
- Evaluate business potential and risks

---

## Solution Architecture

The system follows a Multi-Agent Architecture:

```text
UserProxyAgent
      |
      v
 QueryAgent
      |
      v
AnalyticsAgent
      |
      +----------------+
      |                |
      v                v
ReportAgent      CriticAgent
      |
      v
OutputAgent
```

### Agent Responsibilities

#### QueryAgent

- Retrieves competitor information
- Performs search and location-based discovery
- Collects store-level data

#### AnalyticsAgent

- Calculates footfall metrics
- Identifies top-performing stores
- Generates statistical summaries
- Performs location-based filtering

#### ReportAgent

- Generates textual reports
- Creates tabular summaries
- Produces visual analytics

#### OutputAgent

- Exports results
- Generates CSV reports
- Generates Excel reports
- Returns structured outputs

#### CriticAgent

- Validates collected data
- Detects anomalies
- Identifies missing values
- Flags outliers

#### UserProxyAgent

- Orchestrates the complete workflow
- Maintains conversation flow
- Coordinates agent interactions

---

## Features

- Multi-Agent Workflow using LangGraph
- Competitor Discovery
- Footfall Analysis
- Peak Traffic Identification
- Report Generation
- CSV Export
- Excel Export
- Data Validation
- Conversational Query Interface
- Geospatial Analysis

---

## Technology Stack

| Component | Technology |
|------------|------------|
| Agent Framework | LangGraph |
| LLM Framework | LangChain |
| Language Model | OpenAI GPT |
| Search Tool | Tavily Search |
| Geospatial Analysis | OSMnx |
| Data Processing | Pandas |
| Visualization | Matplotlib |
| Statistical Analysis | NumPy |
| Notebook Environment | Google Colab |

---

## Installation

### Clone Repository

```bash
git clone https://github.com/<your-github-username>/LangGraph-Competitive-Footfall-Insights.git

cd LangGraph-Competitive-Footfall-Insights
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Environment Variables

Create a `.env` file:

```env
OPENAI_API_KEY=your_openai_api_key
TAVILY_API_KEY=your_tavily_api_key
```

---

## Running the Project

Open the notebook:

```bash
jupyter notebook
```

or

```bash
jupyter lab
```

Run:

```text
C13_M4_L9_Project_LangGraph_Competitive_Footfall_Insights.ipynb
```

---


## Future Enhancements

- Real-time footfall APIs
- Interactive dashboard
- Streamlit deployment
- Competitor trend forecasting
- Sentiment analysis from reviews
- Location recommendation engine

---

## Learning Outcomes

- LangGraph Agent Orchestration
- Multi-Agent System Design
- Geospatial Analytics
- LLM Tool Integration
- Data Validation Pipelines
- Business Intelligence Automation

---

## Author

### Antony Pradeep Raj

**ERP Product Manager | Aspiring AI Product Manager**

With nearly 20 years of experience in ERP Product Management, Business Process Automation, and Digital Transformation, I am currently expanding my expertise into Generative AI, Retrieval-Augmented Generation (RAG), AI Agents, and AI Product Management.

GitHub: https://github.com/antonypradeep54
