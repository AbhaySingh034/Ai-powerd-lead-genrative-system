<div align="center">
<p align="center">
  <a href="https://brightdata.com/">
    <img src="https://mintlify.s3.us-west-1.amazonaws.com/brightdata/logo/light.svg" width="300" alt="Bright Data Logo">
  </a>
</p>

# AI-Powered Lead Generation Agent

A next-gen lead generation tool that uses Bright Data to scrape fresh B2B contact data, and OpenAI to qualify, enrich, and provide outreach strategies—all within a seamless Streamlit UI.

<img src="https://img.shields.io/badge/python-3.9+-blue" /> <img src="https://img.shields.io/badge/OpenAI-API-blueviolet" /> <img src="https://img.shields.io/badge/License-MIT-blue" />

<img src="https://media.brightdata.com/2025/09/image-78.png" />
</div>

---

## Features

- 🕵️‍♂️ **Automated Web Scraping:** Instantly collect fresh leads from sources like LinkedIn via Bright Data’s scraping API.
- 📈 **AI-Powered Qualification:** Analyze, score, and enrich leads using OpenAI—no more manual guesswork or lost prospects.
- 💡 **Natural Language Input:** Just describe your ideal lead; the agent extracts structured filters and runs the full workflow.
- 🤝 **Outreach Suggestions:** Get ready-made, personalized tips for email or LinkedIn engagement, tailored per lead.
- 🖥 **Interactive UI:** Manage the pipeline and settings from a user-friendly Streamlit dashboard.

---

## Prerequisites

- Python 3.9+
- [Bright Data Account](https://brightdata.com/) (with API token)
- [OpenAI API Key](https://platform.openai.com/api-keys)
- [Streamlit](https://streamlit.io/) installed
- [Bright Data Datasets access](https://docs.brightdata.com/api-reference/datasets)
- (Optional) dotenv for easier API key management

---

## Installation

1. **Clone the repository**
   ~~~bash
   git clone <repository-url>
   cd ai-leadgen-agent
   ~~~

2. **Create and activate a Python virtual environment**
   ~~~bash
   python -m venv venv
   # macOS/Linux: source venv/bin/activate
   # Windows: venv\Scripts\activate
   ~~~

3. **Install dependencies**
   ~~~bash
   pip install -r requirements.txt
   ~~~

4. **Set API credentials**
   - Create a `.env` file:
     ~~~env
     OPENAI_API_KEY=your_openai_api_key_here
     BRIGHT_DATA_API_KEY=your_bright_data_api_key_here
     ~~~
   - Or, enter them directly in the Streamlit sidebar.

---

## Usage

1. **Launch the application**
   ~~~bash
   streamlit run app.py
   ~~~

2. **Open in your browser**
   - Visit `http://localhost:8501` (auto-opens)

3. **Describe your lead**
   - Enter a natural language query like:  
     `Find marketing managers in fintech companies in Kenya.`
   - Click **Generate Leads**.

4. **Review enriched results**
   - See fully scored, ranked, and enriched leads.
   - Each lead features an AI summary, relevance score, and outreach tip.

---

## How It Works

1. **Natural Language Query:** Just type your requirements (role, industry, location, etc.).
2. **Filter Extraction:** System uses OpenAI to parse and transform your query into APIs filters.
3. **Lead Data Collection:** Bright Data’s API triggers a targeted scrape (e.g., LinkedIn Jobs or Profiles).
4. **AI Enrichment:** Each lead is sent to OpenAI for analysis: scoring, summarizing, and suggesting best engagement channels.
5. **Interactive Exploration:** All results are shown in Streamlit with user-friendly cards and visualizations.

---

## Output Features

- **AI-Scored Leads:** Immediate ranking and insights—no spreadsheets needed!
- **Relevance & Outreach Tips:** For every lead, see why it’s a match and how to engage.
- **Customizable Workflow:** Adjust number of leads, enrichment depth, or tweak the prompt for your ICP.
- **Debug Mode:** Trace each decision and API call for full transparency.

---

## Configuration

### .env file  
Keep your API keys secure:
~~~env
OPENAI_API_KEY=your_openai_api_key_here
BRIGHT_DATA_API_KEY=your_bright_data_api_key_here
~~~

### Sidebar Settings
- **Bright Data API Key:** Paste key (or .env)
- **OpenAI API Key:** Paste key (or .env)
- **Model Selector:** e.g., GPT-3.5, GPT-4O, etc.
- **Max Leads:** Set number of leads to fetch (default: 10)

---

## Troubleshooting

- **No Leads Found**
  - Check API keys and dataset access
  - Relax your search filters (role, location, etc.)
  - Debug mode gives detailed errors

- **Enrichment Fails**
  - Make sure your OpenAI API Key is valid and not rate limited
  - Review API and network connectivity

- **Bright Data Errors**
  - Ensure your token has correct permissions
  - Review [Bright Data documentation](https://docs.brightdata.com/introduction)

---

## License

This project is for educational and internal demo purposes.

---

## Learn More

- [How Bright Data Datasets work](https://docs.brightdata.com/api-reference/datasets)
- [Streamlit Documentation](https://docs.streamlit.io/)
- [OpenAI Platform Docs](https://platform.openai.com/docs)

---

**Ready to supercharge your sales prospecting? Spin up your own AI-Powered Lead Generation Agent and turn manual lead searches into instant, qualified opportunities!**

<p align="center">
  <a href="https://brightdata.com/cp/start" target="_blank" style="text-decoration:none;">
    <img src="https://img.shields.io/badge/Get%20Started-%233D7FFC?style=for-the-badge&logo=rocket&logoColor=white" alt="Get Started" style="height: 48px; border-radius: 8px;">
  </a>
</p>

---



**Made with ❤️ using Bright Data & OpenAI**
