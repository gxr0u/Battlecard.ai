# 🚀 Battlecard.ai — Automated Sales Intelligence Agent

**Battlecard.ai** is an autonomous AI agent designed to revolutionize competitive research. By combining modern web scraping with local Large Language Models (LLMs), it researches companies, extracts product features/pricing, and generates strategic "Sales Battlecards" to help teams win more deals.



## ✨ Key Features

- **Smart-Fetch Technology**: A hybrid scraper that uses `BeautifulSoup` for speed but automatically escalates to `Playwright` (Headless Chromium) for JavaScript-heavy Single Page Applications (SPAs).
- **Intelligent Link Filtering**: Instead of "scraping everything," an agentic loop analyzes the site map to pick the most high-value pages (e.g., `/pricing`, `/features`).
- **FIA Strategy Framework**: Generates insights using the professional **Fact-Impact-Act** framework, providing actionable "trap-setting" questions for sales calls.
- **Privacy-First (Local LLM)**: Powered by **Ollama**, ensuring all competitive data stays on your local machine and never hits a third-party cloud.

## 🛠️ Tech Stack

- **Orchestration**: Python 3.11+
- **LLM Engine**: [Ollama](https://ollama.com/) (Running Qwen 2.5 3B)
- **Scraping**: Playwright & BeautifulSoup4
- **Formatting**: Markdown & IPython

## ⚙️ Configuration & Setup

### 1. Prerequisites
Ensure you have **Ollama** installed and running on your machine.
```bash
ollama pull qwen2.5:3b
