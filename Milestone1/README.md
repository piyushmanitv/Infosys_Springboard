Infosys_Springboard — Milestone 1: Code Explainer



Project Overview

This repository contains the implementation for Milestone 1 of the Infosys CodeGenie AI Explainer and Code Generator Internship Project.
The objective of this milestone is to develop a Code Explainer pipeline that parses, analyzes, and represents Python code snippets using Natural Language Processing (NLP) and Transformer-based models for semantic understanding.




Objectives



1) Parse at least 10 Python code snippets to extract key structural elements.

2) Perform AST (Abstract Syntax Tree) parsing to identify functions, classes, imports, and syntax patterns.

3) Tokenize and analyze the snippets for keywords, operators, and token distribution.

4) Generate embeddings using three pretrained NLP models:

-> MiniLM

-> DistilRoBERTa

-> MPNet

5) Compare model embeddings to study semantic differences in code representation.

6) Visualize and summarize all results through charts and tables.




Pipeline Architecture



🔹 Section 1: Importing Dependencies

Imported all required libraries for:

-> Text preprocessing → re, tokenize, ast

-> NLP & embeddings → sentence_transformers, transformers

-> Visualization → matplotlib, seaborn

-> Data handling → pandas, numpy





🔹 Section 2: Dataset Preparation

Prepared a dataset of 10 Python code snippets, covering:

-> Arithmetic operations

-> Conditional logic

-> Loops and recursion

-> String and list manipulations

-> Class and function definitions





🔹 Section 3: AST Parsing

Used Python’s built-in ast module to extract:

-> Function definitions

-> Class structures

-> Import statements

-> Code-level patterns

This step helps in structural understanding before semantic modeling.





🔹 Section 4: Tokenization & Lexical Analysis

Generated:

-> Token counts

-> Keyword and operator frequencies

-> Token distribution histogram

-> Line length analysis

These insights provide the syntactic richness of each snippet.





🔹 Section 5: Model Embeddings

Used SentenceTransformer to generate embeddings for each snippet via:

-> all-MiniLM-L12-v2

-> all-distilroberta-v1

-> all-mpnet-base-v2

Each model captures code semantics in vector form.





🔹 Section 6: Embedding Comparison & Visualization

Performed cosine similarity across snippets and plotted:

-> Token Distribution

-> Line Length Distribution

-> Pairwise Similarity Heatmaps for all three models

These visualizations reveal semantic closeness between code snippets.




🔹 Section 7: Summary Report

Created a structured summary table containing:

-> Total Functions, Classes, Imports

-> Token Counts & Uniqueness

-> Keywords & Operators Used

Displayed using pandas DataFrame for easy interpretation.




Key Visualizations

-> Token Distribution Plot

-> Line Length Distribution

-> Pairwise Similarity Heatmaps for MiniLM, DistilRoBERTa & MPNet

-> Summary Report Table

Each visualization highlights a different layer of code analysis — from syntax to semantics.




Observations & Insights

1) Embedding similarities were consistent across models for functionally related snippets.

2) MPNet provided more stable contextual embeddings compared to MiniLM and DistilRoBERTa.

3) The AST-based structural breakdown enhanced the interpretability of code semantics.

4) The combination of AST parsing + Transformer embeddings gives both syntactic and semantic understanding of code.



Technologies Used

Category	                Tools / Libraries
Language	                      Python
Notebook	                Google Colaboratory
NLP Models	          MiniLM, DistilRoBERTa, MPNet
Visualization	            Matplotlib, Seaborn
Data Handling	              Pandas, NumPy
Parsing	                    AST, Tokenize
Embedding	              SentenceTransformers



Future Scope

1) Integrate CodeT5 or StarCoder for more advanced code understanding.

2) Extend pipeline for code-to-text summarization (AI Explainer).

3) Develop an interactive web app for real-time code explanation.

4) Incorporate attention heatmaps for interpretability analysis.
