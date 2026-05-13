# Multi-Method Data Analysis with Python

A collection of three data analysis tasks demonstrating different techniques applied to real-world business scenarios. Each notebook tackles a distinct problem using a different toolkit: natural language processing, network analysis, and tabular data integration.

## Overview

| Notebook | Topic | Key Libraries |
|----------|-------|---------------|
| `Q1.ipynb` | Customer review sentiment analysis | pandas, NLTK |
| `Q2.ipynb` | Franchise communication network analysis | pandas, NetworkX, PyVis |
| `Q3.ipynb` | Job applicant and hiring data analysis | pandas |

## Tasks

### Q1 — Customer Review Sentiment Analysis
Analyzes customer feedback from a telecommunications company's service reviews.

- Loads and cleans review text (lowercasing, punctuation removal, normalization)
- Tokenizes reviews and removes English stopwords
- Calculates the most frequent words across all reviews
- Adds a `review_length` column for word counts
- Generates a `sentiment_label` (Positive / Negative / Neutral) based on keyword presence

### Q2 — Franchise Communication Network Analysis
Analyzes communication patterns between franchise branches.

- Builds a directed weighted graph from communication records
- Reports nodes, edges, in-degree, and out-degree
- Computes degree centrality and betweenness centrality
- Identifies the most connected branch and the most important bridge branch
- Finds the shortest path between specified franchises
- Produces a static visualization (NetworkX) and an interactive one (PyVis)

### Q3 — Hiring Data Integration and Analysis
Combines three related datasets: applicants, interviews, and departments.

- Merges datasets on shared key columns
- Detects unmatched records and duplicates
- Classifies interview scores into Strong, Average, and Weak
- Creates pivot tables for average interview score by department
- Summarizes applicants by application status
- Reshapes data to compare interview stages

## Requirements

- Python 3.8+
- Jupyter Notebook or JupyterLab

Install dependencies:

```bash
pip install pandas nltk networkx pyvis matplotlib tabulate openpyxl
```

For Q1, download the required NLTK data (handled automatically inside the notebook):

```python
import nltk
nltk.download('stopwords')
nltk.download('punkt')
```

## Usage

1. Clone the repository:
```bash
   git clone https://github.com/username/multi-method-data-analysis-with-python.git
   cd multi-method-data-analysis-with-python
```
2. Place the required input files (Excel datasets) in the project directory.
3. Open any notebook in Jupyter and run the cells in order:
```bash
   jupyter notebook
```

## Project Structure

```
multi-method-data-analysis-with-python/
├── Q1.ipynb          # Customer review sentiment analysis
├── Q2.ipynb          # Franchise network analysis
├── Q3.ipynb          # Hiring data integration
├── data/             # Input Excel files (not included)
└── README.md
```

## Author

Nusrat