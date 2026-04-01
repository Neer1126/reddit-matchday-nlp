# reddit-matchday-nlp
# ⚽ Arsenal Matchday Sentiment Bot

## 📖 Overview
An automated, multi-agent AI system designed to perform real-time sentiment analysis on football fan reactions during live Arsenal matches. This read-only application extracts aggregate community data to map the emotional highs and lows of the fanbase in response to on-pitch events (goals, VAR decisions, full-time results).

## ⚙️ Architecture & Tech Stack
This project operates entirely off-platform and utilizes the following stack:
* **Language:** Python 3.x
* **AI/Orchestration:** LangChain (for multi-agent routing and LLM sentiment scoring)
* **Data Extraction:** PRAW (Python Reddit API Wrapper)
* **Data Processing:** Pandas 

## 🔍 Data Source & Scope
Data is sourced exclusively from public matchday and post-match threads within football-specific communities, primarily **r/Gunners**. 

**Platform Compliance:**
* **Read-Only:** The script strictly extracts public text data and does not interact, post, vote, or modify content on the Reddit platform.
* **Rate Limiting:** Network requests are strictly throttled well below the 60 requests/minute API limit to ensure zero negative impact on platform infrastructure.
* **Privacy:** The application evaluates aggregate community sentiment and does not store personally identifiable information (PII) or user profiles.

## 🚀 Features (In Development)
- [ ] Automated detection of live Matchday threads.
- [ ] Top-level comment extraction bypassing nested replies (`replace_more(limit=0)`).
- [ ] Real-time ingestion into a LangChain sentiment analysis pipeline.
- [ ] Output generation of overall fan sentiment scores.

## 💻 Local Setup & Installation
*(Instructions will be added once the initial data pipeline is complete and API keys are provisioned.)*
