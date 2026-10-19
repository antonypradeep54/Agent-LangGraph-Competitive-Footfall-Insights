# LangGraph Competitive Location Insights

## Overview

Businesses operating in highly competitive retail locations need timely insights into nearby competitors, customer traffic patterns, and peak business hours.

This project demonstrates a multi-agent workflow using LangGraph and LangChain to identify nearby clothing-store competitors, calculate a location-based proxy score from nearby mapped amenities, and generate structured competitor research reports. The score is a geographic proxy, not a measurement of customer visits or actual store footfall.

The workflow combines Large Language Models (LLMs), web search capabilities, OpenStreetMap-based geospatial data, and agent orchestration to support location-based competitor research. Results depend on the coverage and quality of the available map and search data.

---

## Problem Statement

Businesses in competitive retail locations often struggle to monitor market rivals and understand customer traffic dynamics.

Clothing stores located in busy commercial areas face intense competition and require:

- Visibility into nearby competitors
- Location-based competitor discovery
- Nearby-amenity proxy scoring
- Competitive benchmarking
- Location-based market intelligence

This project addresses these challenges through an AI-powered conversational analytics pipeline.

---

## Intended Beneficiaries

### Business Owners & Store Managers

- Identify nearby competitors
- Understand market saturation
- Compare stores using the project's nearby-amenity proxy score
- Improve operational planning

### Marketing & Strategy Teams

- Use competitor research to inform local marketing questions; actual traffic patterns require a separate reliable data source
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

- Calculates a nearby-amenity proxy score for each store
- Ranks stores by that proxy score
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
- Nearby-Amenity Proxy Scoring
- Competitor Location Analysis
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
git clone https://github.com/antonypradeep54/Agent-LangGraph-Competitive-Footfall-Insights.git

cd Agent-LangGraph-Competitive-Footfall-Insights
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


## Data Sources, Validation, and Limitations

The notebook uses mapped clothing-store locations and counts nearby mapped amenities within a buffer to calculate a `footfall_score`. This is a **proxy score based on geographic context**, not observed customer counts, measured footfall, or verified peak-hour traffic. The current workflow does not establish actual visitor volumes or busiest hours.

OpenStreetMap coverage may be incomplete or uneven, and the proxy score depends on the mapped features available for the selected area. The Critic Agent checks for missing values and potential anomalies; it does not independently verify the real-world accuracy of the underlying data. Validate important findings against reliable local sources before using them for business decisions.

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
- Geospatial Analytics and Proxy-Score Design
- LLM Tool Integration
- Data Validation Pipelines
- Business Intelligence Automation

---

## Author

### Antony Pradeep Raj

**ERP Product Manager | Aspiring AI Product Manager**

With nearly 20 years of experience in ERP Product Management, Business Process Automation, and Digital Transformation, I am currently expanding my expertise into Generative AI, Retrieval-Augmented Generation (RAG), AI Agents, and AI Product Management.

GitHub: https://github.com/antonypradeep54
