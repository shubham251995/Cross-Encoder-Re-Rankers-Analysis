Cross-Encoder Re-Rankers Analysis
Overview
This repository presents a comprehensive study on the effectiveness of cross-encoder re-rankers in the domain of Information Retrieval, particularly using the MS MARCO dataset. Cross-encoder re-rankers, leveraging models like BERT and RoBERTa, are pivotal in enhancing the accuracy of top-quantum rankings in search engines. This research explores the customization of these models for specific tasks to optimize performance.

Models Evaluated
cross-encoder/ms-marco-MiniLM-L-2-v2: A MiniLM model optimized for compact size and speed while maintaining robust language comprehension.
cross-encoder/ms-marco-TinyBERT-L-2-v2: A TinyBERT model adjusted for practical deployment with maintained performance.
distilroberta-base: A distilled version of RoBERTa focusing on efficient performance in constrained environments.
MiniLM-L12-H384-uncased: A lightweight model with a 12-layer architecture designed for rapid processing with minimal computational overhead.
Experiment Setup
The experiment involved fine-tuning and evaluating the above models on the MS MARCO dataset to analyze their relevance scoring abilities between queries and documents. The focus was on enhancing model performance through specific training regimes and fine-tuning methodologies.

Performance Metrics
We utilized metrics such as NDCG@10, Recall@100, and MAP@1000 to measure the effectiveness of each model in real-world scenarios. Detailed discussions are provided on the variations in performance attributed to model architectures, sizes, and training approaches.

Fusion Techniques
Using the Ranx library, several fusion algorithms were tested to enhance retrieval performance by combining results from different models. Techniques like CombMNZ and CombSUM demonstrated significant improvements in ranking precision.

Findings
The analysis highlights the importance of model diversity and strategic training in enhancing the performance of re-rankers. Results indicate that smaller, efficiently trained models can compete with larger models, emphasizing the need for optimized training rather than merely increasing model size.

Usage
Detailed code examples and methodologies are provided in the Jupyter Notebooks within this repository to replicate the experiments and explore the modifications and impacts of various re-ranking strategies.

Contribution
Contributions are welcome! For major changes, please open an issue first to discuss what you would like to change.
