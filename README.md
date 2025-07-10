Recipe Named Entity Recognition with CRF
Project Overview
This project implements a Named Entity Recognition (NER) system using Conditional Random Fields (CRF) to automatically extract ingredients, quantities, and units from unstructured recipe text. The model classifies tokens into predefined categories to create structured recipe data.

Implementation Details
Data
JSON-formatted recipe data with labeled tokens
Each record contains input text and corresponding POS tags
Three entity types: ingredient, quantity, and unit
Project Workflow
Data Preparation

Data validation and cleaning
Train-test split (70:30)
Exploratory Data Analysis

Frequency analysis of ingredients and units
Visualization of top entities
Feature Engineering

Lexical features (token shape, case patterns)
Grammatical features (POS tags, dependency relations)
Domain-specific features (quantity patterns, unit detection)
Contextual features (surrounding tokens)
Model Implementation

CRF with custom feature functions
Class weighting to address imbalance
Hyperparameter tuning
Evaluation

Classification reports for training and validation sets
Confusion matrices
Error analysis
Key Results
The model achieved high accuracy in entity recognition across all three entity types
Strong performance on validation data demonstrates good generalization
Error analysis revealed most misclassifications occur with ambiguous tokens
Technologies Used
Python (sklearn-crfsuite, spaCy, pandas)
Data visualization (matplotlib, seaborn)
NLP techniques (tokenization, POS tagging)
Future Improvements
Enhanced context modeling for ambiguous cases
Incorporating external knowledge sources
Expanding to more diverse recipe formats


**This project was created by Sindhura Peri**
