# ceng463_hw2

This code demonstrates a machine learning pipeline for text classification using transformer models. It includes the following steps:

Data Preparation: The dataset is loaded, preprocessed, and split into training and testing sets. Two text columns (original and English-translated) are prepared for evaluation.
Tokenization: The data is tokenized using a pre-trained tokenizer to transform text into a format suitable for transformer models.
Fine-Tuning: A pre-trained transformer model (e.g., FacebookAI/xlm-roberta-base) is fine-tuned on task-specific labeled data for sequence classification.
Inference: Zero-shot classification using a separate pre-trained model (facebook/bart-large-mnli) is performed on both English-translated and original text without task-specific fine-tuning.
Evaluation: The performance of both fine-tuned and zero-shot models is evaluated using accuracy, precision, recall, and f1-scores. Comparative analysis highlights the strengths and limitations of each approach.
Results: The fine-tuned model achieves superior accuracy and balanced performance across classes, while the zero-shot model demonstrates biases and language dependencies.
This project showcases the advantages of fine-tuning for task-specific performance while offering zero-shot models as a baseline for quick and flexible inference.
