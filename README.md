# Infosys_Springboard


## Approach & Methodology
1. **Load Code Snippets** – 10 diverse Python code examples.  
2. **Parse Code** – Use AST (Abstract Syntax Tree) to extract:
   - Functions  
   - Classes  
   - Imports  
3. **Tokenize Code** – Convert code to tokens, classify into:
   - Keywords  
   - Operators  
   - Identifiers  
   - Others  
4. **Token Patterns & Visualizations** – Analyze frequency of keywords, operators, token types, and line lengths.  
5. **Multi-Model Code Explainer** – Generate context-aware explanations using:
   - MiniLM  
   - DistilRoBERTa  
   - MPNet  
   Compare explanations across models.  
6. **Summary Report** – Aggregate statistics across all snippets.

## Observations
- Keyword `def` is most common due to function definitions.  
- Operators `=` and `+` appear frequently.  
- Token type distribution shows a high percentage of identifiers.  
- Model explanations differ slightly, highlighting different semantic interpretations.  
- Visualizations provide a clear understanding of code patterns.

## How to Run
- Open `Milestone1.ipynb` in [Google Colab](https://colab.research.google.com/).  
- Run all cells sequentially.  
- Visualizations will be generated inline.

## Authors
- Piyushmani Tiwari  
- Contact: piyushmanitiwari500@gmail.com
