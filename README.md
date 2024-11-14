# Overview

The goal of this project is to develop advanced NLP models to automatically generate informative titles for news articles. 
URL of the Kaggle Competiton : https://www.kaggle.com/competitions/inf582-news-articles-title-generation

# Table of Contents

- Project Structure
- Usage
- Data
- Evaluation


# Project Structure

- All the information on the projects are in the NextLP.pdf file
- seq2seq.ipynb contains an exemple of seq2seq model for this problem. This model was not trained due to the lack of data.
- classification_methods.ipynb contains models which give good score by modifying the generation problem in a classification one.
- unsupervised_methods.ipynb contains models which choose the most relevant sentence from the text as a titles
- embeddings_methods.ipynb contains the pretrained models used to embed the sentences
- selection_method_choosing contains our final model which use the embedding of the sentence to generate the title

# Installation

In the beginning of each notebook, the list of required libraries is provided in the first cell where they are imported.


# Usage

In each notebook, you have:
1) The imports of the required libraries
2) The feature extraction
3) The feature reshaping depending on the model used
4) The tokenization of the text
5) The batching of the inputs
6) The description of the model
7) The definition of the hyperparameters and the training
8) The evaluation of the testing datasets

You can execute these different cells in this order and you will get our results.


# Data

We have a JSON files with the texts and their titles to train and evaluate the models. We have a JSON files with just texts for the evaluation on kaggle.



# Evaluation

The performance of our models are assessed using the ROUGE-L F-Score metric. ROUGE is based on the proportion of n-gram overlap between the system-generated sentence and one or more reference sentences.
