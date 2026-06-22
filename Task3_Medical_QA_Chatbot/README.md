# Multi-Modal AI Assistant

## Overview

This project is an AI-powered Multi-Modal Assistant capable of understanding and processing both image and text inputs. It combines computer vision and natural language processing techniques to generate image descriptions, answer user queries, and maintain conversational context for more meaningful interactions.

## Features

* Image upload and processing
* Automatic image caption generation
* Visual question answering based on uploaded images
* Context-aware conversation memory
* Evidence-based and informative responses
* User-friendly interface built with Streamlit

## Technologies Used

* Python
* Streamlit
* Hugging Face Transformers
* BLIP (Bootstrapping Language-Image Pre-training) Model
* Pillow (PIL)

## How to Run

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Start the Application

```bash
streamlit run app.py
```

## System Workflow

```text
User Input (Image + Text)
            ↓
      Image Processing
            ↓
    BLIP Model Analysis
            ↓
 Caption Generation / Q&A
            ↓
 Conversation Memory Update
            ↓
      Response Generation
```

## Key Highlights

* Supports both visual and textual inputs.
* Generates meaningful image descriptions.
* Answers questions related to uploaded images.
* Maintains conversation history for contextual responses.
* Built using state-of-the-art transformer models.

## Future Enhancements

* Multi-image analysis
* Voice input support
* Real-time image recognition
* Advanced multimodal reasoning
* Integration with larger vision-language models

## Author

**Danusree Devasenan**
