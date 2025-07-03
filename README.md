# gemini-financial-decoder
AI-Powered Financial Statement Analyzer using Gemini Pro. Built with Streamlit and Google Gemini Pro LLM, featuring interactive Plotly visualizations and support for CSV/Excel uploads. 

# 📊 Gemini Pro Financial Decoder

Transform your financial analysis with AI-powered insights and interactive visualizations.

An intelligent financial analysis tool that leverages Google's Gemini Pro LLM to automatically analyze balance sheets, profit & loss statements, and cash flow data. Built with Streamlit for an intuitive web interface and modular architecture for easy maintenance.

---

## ✨ Features

- 🤖 **AI-Powered Analysis** – Google Gemini Pro generates intelligent financial insights  
- 📊 **Interactive Visualizations** – Beautiful, dynamic charts and graphs using Plotly  
- 📁 **Multi-Format Support** – Upload CSV and Excel files seamlessly  
- 🔍 **Comprehensive Reports** – Balance Sheet, P&L, and Cash Flow analysis  
- ⚡ **Real-time Processing** – Get insights in seconds  
- 🛡️ **Secure** – Files processed in memory only  

---

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- Google API Key (Gemini Pro)

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/gemini-financial-decoder.git
cd gemini-financial-decoder

# Install dependencies
pip install -r requirements.txt

# Set your API Key
export GOOGLE_API_KEY="your_api_key_here"

# Run the application
streamlit run appfinal.py
```

# Usage
Upload financial statements using the sidebar.

Click "Generate Comprehensive Financial Analysis".

View AI-generated insights and interactive charts.

Optionally, download and save the analysis.

# Supported File Types
.csv
.xlsx, .xls

# Analysis Types
Balance Sheet – Financial health indicators, asset/liability analysis

Profit & Loss – Revenue performance, profitability metrics

Cash Flow – Liquidity and cash management insights

# Technical Architecture

```
┌──────────────┐     ┌──────────────────┐     ┌────────────────────┐
│  Streamlit   │ ───▶│  File Uploader   │ ───▶│   Data Processor    │
│  Interface   │     └──────────────────┘     │     (Pandas)        │
└──────────────┘                               └────────────────────┘
       │                                              │
       ▼                                              ▼
┌──────────────┐     ┌──────────────────┐     ┌────────────────────┐
│  Visualizer  │     │   LLM Handler    │     │  Google Gemini Pro │
│   (Plotly)   │     │   (LangChain)    │     │        API         │
└──────────────┘     └──────────────────┘     └────────────────────┘
```


# Security
No Data Persistence – Files are never stored

Environment-Based API Keys – Use st.secrets or environment variables

Input Validation – Proper handling of formats and file types

Session Isolation – Safe handling for concurrent users

# Performance
🕒 Processes files under 30 seconds (standard size)

📦 Supports files up to 50MB

👥 Optimized for multiple users
