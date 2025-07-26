# Simple-Multilingual-Retrieval-Augmented-Generation-RAG-System

Objective
This project is a simple RAG system that accepts English and Bangla queries. It fetches answers from the HSC26 Bangla 1st Paper PDF using semantic search and generation.
Setup Guide
1. Open the notebook on Google Colab.
2. Run all cells in order.
3. Install necessary libraries (PyMuPDF, langchain, chromadb).
4. Upload and preprocess the HSC26 Bangla 1st Paper PDF.
5. Start querying in Bangla or English.
Tools and Libraries Used
- PyMuPDF
- langchain
- chromadb
- sentence-transformers
- FastAPI 
- Uvicorn 
Sample Queries and Outputs
Q: অনুপমের ভাষায় সুপুরুষ কাকে বলা হয়েছে?
A: শুম্ভুনাথ

Q: কাকে অনুপমের ভাগ্য দেবতা বলে উল্লেখ করা হয়েছে?
A: মামাকে

Q: বিয়ের সময় কল্যাণীর প্রকৃত বয়স কত ছিল?
A: ১৫ বছর
Implementation Questions
1. Used PyMuPDF for PDF text extraction. Faced some formatting issues.
2. Paragraph-based chunking used. Works well for semantic content.
3. Used all-MiniLM-L6-v2 for embeddings. It balances speed and accuracy.
4. Used cosine similarity with ChromaDB for retrieval.
5. Normalized text and maintained short & long-term memory. Vague queries may cause irrelevant output.
6. Results are mostly relevant. Improvement possible with better embeddings or chunking.
Evaluation
- Groundedness: Supported by context
- Relevance: High
- Cosine Similarity: ~0.89
