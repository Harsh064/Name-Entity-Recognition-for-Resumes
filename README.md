# Named-Entity Recognition to Process Resumes

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

            NKNOWN       0.00      0.00      0.00         1
               ame       0.21      0.21      0.21       220
ears of Experience       0.00      0.00      0.00        37
             egree       0.00      0.00      0.00       144
        esignation       0.40      0.19      0.26       430
             kills       0.49      0.62      0.55      4704
      mail Address       0.00      0.00      0.00        76
              mpty       0.95      0.97      0.96    103155
           ocation       0.00      0.00      0.00        73
       ollege Name       0.00      0.00      0.00       214
ompanies worked at       0.27      0.01      0.01       470
    raduation Year       0.00      0.00      0.00        58

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

