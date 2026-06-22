# Medical Q&A Chatbot using MedQuAD

## Overview

The Medical Q&A Chatbot is an AI-powered application developed using the MedQuAD (Medical Question Answering) dataset. The system enables users to ask medical questions and retrieves the most relevant answers through semantic similarity search and basic medical entity recognition techniques.

Built with Python and Streamlit, the chatbot offers an interactive and user-friendly platform for exploring medical information from a trusted dataset.

## Features

* Retrieves relevant answers from the MedQuAD dataset.
* Semantic search using Sentence Transformers.
* Medical entity recognition for:

  * Symptoms
  * Treatments
  * Diagnoses
* Confidence score calculation for retrieved responses.
* Interactive web interface using Streamlit.
* Fast and efficient medical information retrieval.

## Technologies Used

* Python
* Streamlit
* Sentence Transformers
* XML Parsing
* MedQuAD Dataset

## Project Structure

```text id="d3k7q2"
Task3_Medical_QA_Chatbot/
│── app.py
│── chatbot_v3.py
│── REPORT.docx
│── README.md
```

## How to Run the Project

### Install Dependencies

```bash id="r7j2w8"
pip install -r requirements.txt
```

### Run the Application

```bash id="n4z6x1"
streamlit run app.py
```

### Access the Application

Open the local URL displayed in your browser after running the Streamlit application.

## Example Queries

Try asking questions such as:

* breast cancer symptoms
* breast cancer treatment
* melanoma diagnosis
* diabetes symptoms
* hypertension treatment

## System Workflow

```text id="p8m5y4"
User Query
     ↓
Medical Entity Detection
     ↓
Semantic Similarity Search
     ↓
Confidence Score Calculation
     ↓
Relevant Answer Retrieval
     ↓
Response Display
```

## Sample Functionality

The chatbot:

1. Identifies the type of medical query.
2. Detects relevant medical entities.
3. Searches the MedQuAD dataset using semantic similarity techniques.
4. Calculates a confidence score for the match.
5. Returns the most relevant medical question and answer available in the dataset.

## Key Highlights

* AI-powered medical question answering.
* Semantic search for improved retrieval accuracy.
* Basic medical entity recognition.
* Interactive Streamlit-based interface.
* Lightweight and easy-to-use architecture.

## Future Enhancements

* Advanced Named Entity Recognition (NER)
* Multi-language support
* Voice-based medical queries
* Integration with medical knowledge graphs
* Enhanced confidence scoring mechanisms

## Disclaimer

This project is intended solely for educational and research purposes. The information provided is retrieved from the MedQuAD dataset and should not be considered professional medical advice, diagnosis, or treatment. Always consult qualified healthcare professionals regarding medical concerns.

## Author

**Danusree Devasenan**
