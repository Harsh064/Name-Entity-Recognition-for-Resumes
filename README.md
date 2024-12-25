# Named-Entity Recognition to Process Resumes
Colab Link: https://colab.research.google.com/github/Harsh064/Name-Entity-Recognition-for-Resumes/blob/main/Named_Entity_Recognition_For_Resumes.ipynb

## Overview
This project focuses on extracting and classifying key information from resumes, such as:
- Companies the applicant has worked at.
- Skills possessed by the applicant.
- Types of degrees and other relevant details.

By leveraging pre-trained models and tokenizers from the Hugging Face library, we fine-tune a transformer model for the Named-Entity Recognition (NER) task.

## Features
- **Dataset Cleaning**: Prepares and cleans the dataset for better alignment with named entities.
- **Tokenization**: Uses the DistilBERT tokenizer to process sequences efficiently.
- **Model Fine-Tuning**: Fine-tunes a pre-trained transformer model for accurate NER.

## Installation
To run this project, ensure you have the following libraries installed:

```bash
pip install transformers datasets numpy pandas scikit-learn matplotlib tensorflow logging re tqdm collections seqeval
```

## Steps
### 1. Dataset Preparation
- Clean and preprocess the dataset.
- Define categories and tags for named entities.

### 2. Tokenization and Label Alignment
- Tokenize inputs using the DistilBERT tokenizer.
- Align labels with tokens and pad sequences to a standard length.

### 3. Model Training
- Fine-tune a pre-trained transformer model for the NER task.
- Monitor model performance using metrics like precision, recall, and F1-score.

### 4. Evaluation
- Evaluate the model's performance on a validation set.
- Analyze errors and refine the model for better accuracy.

## Results
- The model successfully identifies named entities from resumes.
- Performance metrics:

                    precision    recall  f1-score   support
  
         micro avg       0.93      0.94      0.93    109582
         macro avg       0.19      0.17      0.17    109582
      weighted avg       0.92      0.94      0.93    109582
      
## Libraries Used
- **transformers**
- **scikit-learn**
- **pandas**
- **numpy**
- **matplotlib**
- **tensorflow**
- **logging**
- **re**
- **tqdm**
- **collections**
- **seqeval**

## Acknowledgments
- Hugging Face for the transformers library.
- Open-source datasets for NER tasks.

