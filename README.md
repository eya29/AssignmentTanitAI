# Text Classification with BERT for Reproductive Medicine Research Papers
Overview
This project demonstrates the use of a transformer-based model (BERT) for text classification on a dataset of medical research papers. The dataset contains research papers in the field of reproductive medicine, with the goal of classifying them into predefined categories using an unsupervised learning approach. The project involves:

Data Preprocessing: Cleaning and tokenizing text data.
Modeling: Using BERT (Bidirectional Encoder Representations from Transformers) for feature extraction and classification.
Evaluation: Evaluating the model's performance using accuracy, recall, and F1-score.

Data Preprocessing
The preprocessing pipeline processes the JSON data containing medical research papers into a clean format suitable for model training. It includes:

Loading Data: The data is loaded from JSON files and combined into a single DataFrame.
Text Cleaning: Text is lowercased, non-alphabetic characters are removed, and extra spaces are trimmed.
Tokenization: The text is tokenized using the BERT tokenizer.

Model Training
The model is based on BERT (bert-base-uncased), a pre-trained transformer model that is fine-tuned for sequence classification tasks. The following steps are taken during training:

Model Definition: A custom classification head is added on top of BERT for predicting class labels.
Training Loop: The model is trained using the Adam optimizer and Cross-Entropy Loss.
Data Splitting: The data is split into training, validation, and test sets.

Model Evaluation
Once the model is trained, evaluation is performed using the following metrics:

Accuracy: Measures the percentage of correctly classified instances.
Recall: Measures the model’s ability to identify all relevant instances.
F1-Score: The harmonic mean of precision and recall, providing a balance between the two.
