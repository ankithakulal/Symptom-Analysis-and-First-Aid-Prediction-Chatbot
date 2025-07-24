# Symptom-Analysis-and-First-Aid-Prediction-Chatbot

Machine learning and semantic search–based chatbot that helps users find appropriate first aid solutions based on problem descriptions. It uses natural language processing and similarity matching to provide accurate recommendations.

__📁Project Structure__

- app.py               # Streamlit web app interface

- prediction.py        # Console-based version of the prediction logic

- firstaid.xlsx        # Dataset containing "Problem" and "Solution" pairs


__🧠Technologies Used__

- Python 🐍

- scikit-learn for model training (TF-IDF + Naive Bayes)

- sentence-transformers for semantic similarity

- Streamlit for the web-based interface

- Pandas for data handling

- Torch for tensor operations


__📚 Dataset__

The dataset (firstaid.xlsx) contains two columns:

Problem: Description of the first aid situation.

Solution: The appropriate first aid response.


__🚀 How It Works__

✅ Console Version (prediction.py)
Loads the dataset.

Trains a text classification model (TF-IDF + Naive Bayes).

Also builds semantic embeddings using SentenceTransformer.

Accepts user input in a loop and returns the best-matching solution based on semantic similarity.

✅ Web App Version (app.py)

Uses Streamlit to create an interactive interface.

Accepts problem description through a text box.

Shows predicted first aid solution and similarity score.

Stores recent searches in the sidebar.


__💡 Features__

- Handles free-text problem descriptions

- Uses semantic matching for intelligent prediction

- Gives confidence scores based on similarity

- Stores recent problem searches

- Simple, clean UI with Streamlit

