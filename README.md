Natural language to SQL — ask your business data questions in plain English, get instant charts and insights.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Python 3.11
Streamlit
Ollama · LLM
NLP-to-SQL
RAG
MIT License
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
WHAT IT DOES ?
1.Natural language queries
Type questions like "top 5 products by revenue last quarter" — no SQL needed
2.Instant SQL generation
Locally hosted LLM via Ollama translates intent to precise SQL queries
3.Dynamic visualizations
Auto-rendered charts and tables via Streamlit — bar, line, pie, and more
4.Fully local & private
No data leaves your machine — LLM runs locally via Ollama
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Architecture
User question
→
Schema context (RAG)
→
Ollama LLM
→
SQL query
→
DB execution
→
Streamlit chart
The app injects the database schema as context alongside the user's question, prompting the LLM to generate syntactically correct SQL. Results are rendered dynamically as charts or tables depending on the data shape.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Tech stack
Python  ·  Streamlit  ·  Ollama (LLaMA / Mistral)  ·  SQLite / PostgreSQL  ·  Pandas  ·  Plotly
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Sample queries
These all work out of the box with the included sample retail database:

"Show me total sales by region for Q1 2024"
"Which product category had the highest return rate?"
"List top 10 customers by lifetime value"
"Monthly revenue trend for the last 6 months"
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Results
Deployed at Bahwan Cybertek — enabled 15+ business users to run self-serve analytics, reducing SQL request turnaround from 2 days to under 5 minutes.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Project structure
chatbi-nlp-sql-assistant/
 ├── app/            # Streamlit UI + routing
 ├── pipeline/       # NLP-to-SQL chain, prompt templates
 ├── database/       # Schema loader, query executor
 ├── data/           # Sample datasets (anonymised)
 ├── assets/         # demo.gif, architecture.png
 ├── app.py         # Entry point
 ├── requirements.txt
 └── README.md
Author
Adithya D 
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
