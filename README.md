# Project-02_natural-language-processing
# 🛍️ Customer Support Chatbot for Online Shopping

## 📘 Overview
The **Customer Support Chatbot** is an intelligent virtual assistant designed to handle basic customer queries for an online shopping platform.  
It can respond to questions about **order tracking, return policies, delivery times, product information, refunds**, and more — reducing the need for human support intervention.

This chatbot uses **Natural Language Processing (NLP)** techniques for text preprocessing, **intent classification** using a machine learning model, and **Named Entity Recognition (NER)** for extracting information such as order numbers from user queries.

---

## 🎯 Goal
To build an AI chatbot capable of understanding customer queries and responding accurately using a combination of rule-based logic and ML-powered intent recognition.

---

## 🔑 Concepts Used
- **Intent Recognition** → Classifies query type (e.g., order status, return policy, product info)  
- **Named Entity Recognition (NER)** → Extracts order numbers and product names  
- **Rule-based + Similarity Matching** → Responds using pre-defined templates and TF-IDF similarity  
- **Machine Learning Classifier** → Logistic Regression with TF-IDF Vectorization  

---

## 🧠 Workflow
1. **Preprocess the user query** (tokenization, stopword removal, lemmatization).  
2. **Classify intent** → Detect query type using a trained ML model.  
3. **Extract entities** → Identify order numbers or product references using regex and spaCy NER.  
4. **Generate a response** → Combine rule-based templates and dynamic entity data (e.g., order IDs).  
5. **Use similarity fallback** → Handle unrecognized queries using cosine similarity against stored responses.  

---

## 🧰 Tools & Libraries
- **Python** 🐍  
- **NLTK** for text preprocessing  
- **Scikit-learn** for intent classification  
- **spaCy** for NER and entity extraction  
- **Pandas** for dataset management  

---

## 🗂️ Dataset Example
A small sample dataset of intents and example queries:

| Intent | Example Query | Response |
|--------|----------------|-----------|
| Order Status | Where is my order #12345? | Your order #12345 is out for delivery. |
| Return Policy | How can I return a product? | You can return products within 15 days via our online portal. |
| Product Info | Does this phone support fast charging? | Yes, this phone supports fast charging. |

You can expand this dataset by adding more intents and query variations to improve accuracy.

---
