<img width="825" height="464" alt="image" src="https://github.com/user-attachments/assets/9c86cc53-a514-49cd-8aeb-f093fac141a5" />CodeGenie – Model Benchmarking & Analysis Notebook


Milestone 2 Project | Infosys Springboard AI Internship


1. Project Overview


CodeGenie is an interactive Jupyter/Colab-based system designed to benchmark and analyze multiple AI code generation models on programming prompts. It provides intuitive visual UIs using ipywidgets and powerful metric-based evaluations for code quality, maintainability, and generation performance. This project demonstrates the ability to run, compare, and visualize performance across various language models under consistent test conditions.

Key Features

• Benchmark all models at once or selectively inspect specific ones.
• Calculates advanced code metrics such as Cyclomatic complexity, Maintainability index, and generation time per model.
• Clean tabular results and comparative plots.
• Exportable logs for session analysis.
• Works seamlessly in Google Colab and Jupyter Notebook.


Technologies Used


<img width="730" height="325" alt="image" src="https://github.com/user-attachments/assets/95076ce9-2d20-4707-aac1-8f52626cf9bd" />


2. Environment Setup


Follow the steps below to set up your environment:

1. Open the notebook in Google Colab and enable GPU runtime for better performance.
2. Install dependencies using the command:
  •	!pip install transformers torch accelerate radon matplotlib ipywidgets



3. Hugging Face Authentication

  
1. Visit https://huggingface.co/ and create an account.
2. Navigate to Profile → Settings → Access Tokens and generate a token.
3. Use the token in the Colab notebook for model authentication.



4. User Interface Overview


The notebook includes an interactive UI built using ipywidgets. It allows users to select AI models via checkboxes, enter code prompts, and visualize comparative results of generated code snippets.


Figure 1: Snapshot of the interactive benchmarking UI.

<img width="1723" height="533" alt="image" src="https://github.com/user-attachments/assets/1036d0d0-ec32-4de3-b8c5-e8a0763cadba" />


Figure 2: Snapshot of the interactive benchmarking UI.

<img width="1773" height="744" alt="image" src="https://github.com/user-attachments/assets/9719e2f9-19f6-4020-b963-aaafaf43545d" />




5. Model Evaluation Metrics


Each model was evaluated on three key parameters to quantify performance differences.


<img width="738" height="254" alt="image" src="https://github.com/user-attachments/assets/823af298-5a9c-4fc9-91f9-81b026287444" />



6. Comparative Model Analysis


The benchmarking compared the outputs of Gemma-2B-IT, DeepSeek-Coder-1.3B, and StableCode. Each model was tested with identical prompts to evaluate output consistency and efficiency.
  - Gemma-2B-IT: Balanced output with strong readability and efficient structure.
  - DeepSeek-Coder-1.3B: High maintainability index and concise logic.
  - StableCode: Produced minimal lines of code but slightly reduced readability.



7. Visualization


The results were visualized using matplotlib graphs showing variation across metrics like complexity, maintainability, and LOC. These visualizations helped in identifying trade-offs between code compactness and readability.


8. Results and Insights

  
1. Gemma-2B-IT achieved the best balance between readability and complexity.
2. DeepSeek-Coder-1.3B performed best in maintainability.
3. StableCode optimized for brevity but required manual review for clarity.
4. Visualization confirmed that a balance between readability and compactness leads to better software maintainability.


9. Conclusion

   
This milestone highlights that code generation models exhibit distinct trade-offs. Gemma-2B-IT and DeepSeek-Coder-1.3B were the top-performing models due to their balanced output quality. StableCode, though efficient, showed a need for refinement in readability.



10. References


• Hugging Face Transformers Documentation
• Radon Documentation for Code Metrics
• Infosys CodeGenie Documents
• Google Colab Documentation



Example Output Summary


Model	              Prompt	              Complexity	        Maintainability	        Gen Time (s)
GPT-2  	      Fibonacci Series	            5.0                  	78.2	                  1.34
CodeGen	      Factorial Program	            3.0	                  85.7	                  0.98


Future Enhancements


• Integrate LLM evaluation metrics like BLEU or CodeBLEU.
• Add syntax error detection with AST parsing.
• Allow CSV export of all results automatically.
• Add multi-threaded prompt execution for faster comparisons.


Author


Piyushmani Tiwari
B.Tech (Information Technology) — Government Engineering College, Bilaspur

Email: piyushmanitiwari500@gmail.com

GitHub: https://github.com/piyushmanitv

LinkedIn: https://linkedin.com/in/piyushmani-tiwari-2349101a9



License


This project is released under the MIT License, allowing open collaboration and modification for educational use.

