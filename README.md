# RAG_project
A Retrieval-Augmented Generation (RAG) system that answers natural language questions about retail sales data using vector embeddings and LLMs.

## Instructions

### 1. Download Data
```
Download: Superstore.csv from https://www.kaggle.com/datasets/vivek468/superstore-dataset-final
```
### 2. Install Dependencies
```
pip install -r requirments.txt
```
### 3. Build Vector Database (Local)
```
Run: preprocess.ipynp
Output: analysis.pkl file
```
```
Run: vector_db.ipynb
Output: chroma_db folder
```
### 4. Deploy to Colab
```
zip -r Files.zip chroma_db
```
```
Open: RAG_pipeline_COLAB.ipynb in Google Colab
Upload: Files.zip
Add: your Grok API key from https://console.groq
Run: all cells to test the sales queries
Supported queries are in analysis.txt.