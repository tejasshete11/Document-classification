# Document-classification
# 📄 Document Classification using NLP Techniques

## 📌 Project Overview
This project demonstrates **document classification** using Natural Language Processing (NLP).  
The objective is to classify text documents into categories by applying preprocessing, feature extraction, and machine learning algorithms.
This project demonstrates the complete pipeline of building a document classification system:
- Text preprocessing
- Feature extraction
- Model training
- Evaluation

---

## 📊 Dataset
- The dataset consists of a collection of text documents, each labeled with a **category**.  
- Categories may represent topics, sentiments, or subject domains.  
- Before training, we analyze the dataset with:
 - **Shape of dataset ** `(2225, 2)` 
  - **Category distribution** → To check if the dataset is balanced or imbalanced  

---

## 🛠️ Preprocessing
Raw text data cannot be fed directly into machine learning models.  
Therefore, preprocessing is necessary to remove noise and standardize the data.  
Steps applied to clean and prepare the text data:
1. **Lowercasing** → Makes the text uniform (e.g., "Apple" and "apple" are treated the same).  
2. **Removing punctuation and numbers** → These do not contribute to semantic meaning.  
3. **Tokenization** → Splits text into individual words (tokens).  
4. **Stopword removal** → Eliminates common words (like "is", "the", "and") which don’t add much meaning.  
5. **Lemmatization** → Converts words to their root form (e.g., "running" → "run").  

These steps help reduce noise, standardize the text, and improve model performance.5. Lemmatize tokens  

---

## 🔍 Feature Extraction
Since machine learning models work with **numerical data**, text must be converted into numeric vectors.  
- **TF-IDF (Term Frequency – Inverse Document Frequency)** → Assigns weights to words based on how frequently they appear in a document compared to the whole dataset. This gives higher importance to rare but meaningful words.  

---

## 🤖 Models Used
Three popular machine learning algorithms were implemented:

1. **Naive Bayes**  
   - Based on Bayes’ theorem.  
   - Works very well for text classification because of the “bag of words” assumption (features are conditionally independent).  
   - Fast, simple, and often a strong baseline.  

2. **Logistic Regression**  
   - A linear model that estimates probabilities of classes.  
   - Good for high-dimensional sparse data such as TF-IDF features.  
   - Provides strong performance with relatively low complexity.  

3. **Support Vector Machine (SVM)**  
   - Finds the hyperplane that best separates categories in feature space.  
   - Particularly effective in high-dimensional spaces (like text data).  
   - Often achieves high accuracy in NLP tasks.  

---

## 📈 Model Evaluation
Models were evaluated using:
- **Accuracy** → Percentage of correct predictions.  
- **Precision, Recall, and F1-score** → Provide deeper insight into model performance on each class.  
- **Confusion Matrix** → Visualizes where the model is making correct and incorrect predictions.  

---

## 📈 Results
Performance was evaluated using **Accuracy** and **Classification Report (Precision, Recall, F1-score)**.  

- Naive Bayes → Accuracy: `98%`  
- Logistic Regression → Accuracy: `98%`  
- SVM → Accuracy: `98%`  

---
