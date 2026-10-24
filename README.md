# AI Data Analyst

Ask questions about your data in plain English. Upload a CSV or Excel file and an AI agent explores it for you — writing and running real SQL against your table and answering with the actual numbers, not guesses.

## What it does

- Upload any `.csv` or `.xlsx` file and preview it instantly
- Ask questions the way you would ask a colleague: *"Which region had the highest sales last quarter?"*
- The agent plans the query, runs it on DuckDB, and explains the result in clear language
- Works on churn data, sales sheets, survey results, exports from any tool

## Tech stack

- **Streamlit** — web UI
- **Agno** — agent framework
- **Google Gemini 2.5 Flash** — reasoning model
- **DuckDB + Pandas** — in-memory SQL analytics over the uploaded file

## Run it locally

```bash
pip install -r requirements.txt
streamlit run ai_data_analyst.py
```

Open the app, paste your Google Gemini API key in the sidebar (free from Google AI Studio), upload a file, and start asking.

## Example questions

- "What are the top 5 products by revenue?"
- "Show monthly signups for the last year — is there a trend?"
- "Which customers churned, and what do they have in common?"

## Author

**Abdul Wahid** — AI/ML Developer
[Portfolio](https://www.abdulwahid.me) · [GitHub](https://github.com/abduIwahid) · [LinkedIn](https://www.linkedin.com/in/abdu1wahid)

## Credits

Adapted from a template in the [awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) collection by Shubham Saboo, and reworked to run on Gemini instead of OpenAI. Licensed under Apache-2.0 — see [LICENSE](LICENSE).
