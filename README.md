# open-llm-metrics-pipeline
A simple Python & SQLite ETL pipeline that ingests, cleans, and analyzes public Open LLM evaluation benchmarks from Hugging Face.

📁 Project Structure
```
open-llm-metrics-pipeline/
│
├── .gitignore              # Specifies intentionally untracked files to ignore (venv, *.db, cache)
├── requirements.txt        # Third-party Python dependencies (e.g., requests)
├── README.md               # Project overview, architecture diagram, and setup instructions
│
├── data/
│   └── .gitkeep            # Keeps the data folder in version control for SQLite database / raw output
│
├── src/
│   ├── __init__.py         # Marks the directory as a Python package
│   ├── extract.py          # Data ingestion from Hugging Face API
│   ├── transform.py        # Data cleaning, normalization, and metric calculations
│   └── load.py             # SQLite database connection, table creation, and data persistence
│
└── main.py                 # Pipeline orchestrator (runs Extract -> Transform -> Load)
```
