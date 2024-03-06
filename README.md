# NER with Hugging Face Transformers

## Project Overview

In this project, we aimed to train an NER classifier for the task “Emerging and Rare entity recognition” from the Workshop on Noisy User-generated Text [(W-NUT)](https://noisy-text.github.io/2017/emerging-rare-entities.html). The W-NUT dataset features annotations in IOB format across various named entity types within noisy text. The primary objectives include data preprocessing, hyperparameter optimization, training a sequence labeling model using Hugging Face Transformers, and evaluating the model using suitable evaluation metrics. Our approach includes fine-tuning a pre-trained BERT model, data preprocessing, and hyperparameter optimization.

## Technical Approach

1. **Data Preprocessing:** Adjusting dataset format for Transformers library compatibility, focusing on tokenization and label alignment.
2. **Model Selection and Training:** Utilizing `bert-base-cased` for its efficiency, with a fine-tuning approach tailored to the dataset.
3. **Hyperparameter Optimization:** Experimenting with various parameters to enhance model performance significantly.

## Experimental Results

The model that performed the best, based on the F1-score, was trained using a learning rate of 1e-6  and a batch size of 8. It achieved a 56.40% F1-score on the validation dataset. Our work led to better precision, recall, and F1-score on the test set, as indicated in the following table.

| Model           | Precision | Recall | F1    |
|-----------------|-----------|--------|-------|
| Baseline        | 0.566     | 0.333  | 0.420 |
| Optimized model | 0.580     | 0.349  | 0.436 |

For an in-depth analysis of our conclusions and a complete set of results, please refer to the detailed report provided.

