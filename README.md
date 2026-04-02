# SmartTrip: AI-Powered Destination & Accommodation Recommender

## Overview
SmartTrip is an AI-powered tourism recommendation system that generates personalized travel destination and accommodation suggestions based on user-provided natural language input.

The system combines semantic embeddings (Sentence-BERT) with traditional machine learning techniques to deliver context-aware and interpretable recommendations.

---

## Key Features
- Free-text based destination recommendation
- Semantic understanding using Sentence-BERT
- Linear SVM for multi-class destination prediction
- Top-3 destination recommendation output
- Explainable predictions based on user input sentences
- Accommodation recommendation using cosine similarity
- Budget-based filtering using K-Means clustering

---

## System Workflow
1. User inputs travel preferences in natural language  
2. Input is processed using sentence-level embeddings  
3. Linear SVM predicts top 3 destinations  
4. Explainability highlights which input sentences influenced predictions  
5. Accommodation module:
   - Filters by predicted destinations  
   - Applies budget clustering (K-Means)  
   - Uses cosine similarity to rank hotels  

---

## Dataset

### Destination Dataset
- ~1000+ entries  
- 9 destination classes  
- Paragraph-level travel descriptions  
- Augmented to balance class distribution  

### Accommodation Dataset
- ~500 entries  
- Hotel descriptions collected from TripAdvisor  
- Includes price, location, and metadata  

---

## Models & Techniques
- Sentence-BERT (all-MiniLM-L6-v2) for semantic embeddings  
- Linear SVM for destination classification  
- Stratified 5-Fold Cross-Validation for model evaluation  
- Top-K Accuracy (Top-3) for recommendation effectiveness  
- K-Means Clustering (Elbow Method) for budget segmentation  
- Cosine Similarity for accommodation ranking  

---

## Evaluation
- Cross-validation accuracy (SVM): **0.8338**  
- Top-3 accuracy: **0.917**  
- Evaluation is based on technical performance metrics  

---

## Note
This project focuses on backend recommendation logic and model development. A graphical user interface (UI) was not implemented.

---

## How to Run
- Open the notebook in Google Colab  
- Install required libraries  
- Run all cells sequentially  
- Provide input when prompted  

---

## Project Type
Final Year Research Project  
AI-Powered Tourism Recommendation System
