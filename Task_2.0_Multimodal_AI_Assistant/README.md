# Multi-Modal AI Assistant

## Overview

The Multi-Modal AI Assistant is an intelligent application capable of understanding and processing both image and text inputs. By combining computer vision and natural language processing techniques, the assistant can generate image captions, answer questions related to uploaded images, and maintain conversational context for enhanced user interaction.

The project is built using Python, Streamlit, and the BLIP (Bootstrapping Language-Image Pre-training) model from Hugging Face Transformers.

## Features

* Image upload and analysis
* Automatic image caption generation
* Visual question answering (VQA)
* Conversation memory for contextual interactions
* Evidence-based response generation
* Interactive and user-friendly Streamlit interface

## Technologies Used

* Python
* Streamlit
* Hugging Face Transformers
* BLIP Model
* Pillow (PIL)

## Project Structure

```text
Multi_Modal_AI_Assistant/
│── app.py
│── requirements.txt
│── README.md
│── images/
│── models/
```

## How to Run

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Launch the Application

```bash
streamlit run app.py
```

### Access the Application

After running the command, open the local URL displayed in your browser.

## System Workflow

```text
Image/Text Input
        ↓
Data Processing
        ↓
BLIP Model Analysis
        ↓
Caption Generation / Question Answering
        ↓
Conversation Memory Update
        ↓
Response Generation
```

## Key Functionalities

### Image Caption Generation

The assistant automatically generates descriptive captions for uploaded images.

### Visual Question Answering

Users can ask questions about an uploaded image, and the system provides relevant answers based on the image content.

### Conversation Memory

The chatbot maintains context across interactions, enabling more natural and coherent conversations.

### Evidence-Based Responses

Responses are generated using information extracted from image analysis and user queries.

## Future Enhancements

* Voice input and output support
* Real-time image recognition
* Multi-image analysis
* Advanced multimodal reasoning
* Integration with large vision-language models (VLMs)

## Author

**Danusree Devasenan**
