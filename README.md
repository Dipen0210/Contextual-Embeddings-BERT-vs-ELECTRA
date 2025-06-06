# Contextualized Word Embeddings: Comparison of ELECTRA and BERT Models

## Project Overview

This project explores the concept of contextual word embeddings, comparing how different models (ELECTRA and BERT) perform in generating word embeddings, particularly focusing on their ability to disambiguate words based on context. The project implements and evaluates the effectiveness of contextual embeddings generated by the ELECTRA model, comparing them against BERT’s embeddings. Additionally, performance metrics such as speed and efficiency are examined for both models.

## Project Structure

This project is divided into two main parts:

### Part 1: Contextual Word Embedding with Same Word, Different Meaning

- **Objective**: Visualize how the meaning of the same word changes based on context. The example used is the word "bank," which has different meanings in two sentences.
- **Methodology**: 
    1. Load the ELECTRA model and tokenizer from Hugging Face's Transformers library.
    2. Tokenize input sentences and generate embeddings.
    3. Perform dimensionality reduction using t-SNE to visualize embeddings.
    4. Compare token embeddings in the two contexts of the word "bank."

### Part 2: Paragraph Testing - BERT vs. ELECTRA

- **Objective**: Compare the speed and effectiveness of BERT and ELECTRA models in generating contextual embeddings for a paragraph.
- **Methodology**:
    1. Load both the BERT-base and ELECTRA-small models.
    2. Run both models on GPU.
    3. Measure and compare the time taken to generate embeddings for the same input paragraph.
    4. Visualize the embeddings using t-SNE for comparison.

## Requirements

- Python 3.x
- PyTorch
- Hugging Face's Transformers library
- Matplotlib (for visualization)
- NumPy (for handling array operations)
- scikit-learn (for t-SNE)
