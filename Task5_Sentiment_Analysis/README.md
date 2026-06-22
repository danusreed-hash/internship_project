# Sentiment-Aware Customer Support Chatbot

## Overview

This project is an AI-powered customer support chatbot that detects user sentiment during conversations and adapts its responses accordingly. The chatbot provides empathetic, appreciative, or neutral responses based on customer emotions while maintaining multilingual support across English, Hindi, Spanish, and French.

## Features

* Sentiment analysis for positive, negative, and neutral customer messages.
* Emotion-aware responses that adapt to user sentiment.
* Automatic language detection for English, Hindi, Spanish, and French.
* Mixed-language conversation support using language hints and Unicode script detection.
* Intent recognition for greetings, ticket booking, weather inquiries, status checking, cancellations, and appreciation messages.
* Session-based context memory for maintaining conversational continuity.
* Language switching within the same conversation.
* Interactive browser-based chat interface displaying language, intent, sentiment score, engine type, and turn count.
* Lightweight Python backend built using only standard library modules.
* Optional OpenRouter API integration for enhanced reasoning and response generation.

## Technologies Used

* Python
* HTML
* CSS
* JavaScript
* OpenRouter API
* Standard Python Libraries

## How to Run

Navigate to the project directory:

```bash
cd multilingual_chatbot
```

Start the application:

```bash
python app.py
```

Open the application in your browser:

```text
http://127.0.0.1:8000
```

## Running Tests

```bash
python tests.py
```

The test suite validates sentiment classification accuracy across positive, negative, and neutral examples.

## OpenRouter Online Mode

### Option 1: Configure Through the Application

1. Launch the application.
2. Open `http://127.0.0.1:8000`.
3. Enter your OpenRouter API key.
4. Keep the model as `openrouter/auto` or specify another model.
5. Click **Save API Key**.

### Option 2: Configure Using Environment Variables

```env
OPENROUTER_API_KEY=your-api-key
OPENROUTER_MODEL=openrouter/auto
```

Restart the application:

```bash
python app.py
```

When configured correctly, the chatbot uses OpenRouter's OpenAI-compatible Chat Completion API. If the API is unavailable or configuration fails, the application automatically switches to the offline rule-based engine.

## Sample Conversation

### Positive Sentiment

**User:** Thanks, this service is really helpful!

**Detected Sentiment:** Positive

**Bot:** I'm glad this is helping you. You're welcome, and I'll keep the conversation context ready for your next message.

### Negative Sentiment

**User:** I am frustrated because my ticket is delayed and nobody helped me.

**Detected Sentiment:** Negative

**Bot:** I'm sorry you've had this experience. I understand your frustration and will help resolve the issue as quickly as possible.

### Neutral Sentiment

**User:** What is the status of booking ID 4821?

**Detected Sentiment:** Neutral

**Bot:** I understand you want to check the booking status. Please provide your booking or tracking ID.

## System Workflow

```text
User Message
      ↓
Language Detection
      ↓
Sentiment Analysis
      ↓
Intent Detection
      ↓
Entity Extraction
      ↓
Conversation State Update
      ↓
Emotion-Aware Response Generation
```

## Stored Conversation Context

The chatbot maintains:

* Preferred language
* Previous intent
* Previous sentiment analysis
* Extracted entities such as destination, date, time, and travel mode
* Complete conversation history

## Evaluation Criteria

### Accuracy

Run the test suite to verify sentiment classification performance across positive, negative, and neutral examples.

### Response Appropriateness

Ensure negative customer messages receive empathetic responses before task-specific assistance.

### Customer Experience

Compare traditional responses with sentiment-aware responses to evaluate improvements in conversational quality and user satisfaction.

## Key Highlights

* Emotion-aware customer support interactions.
* Multilingual conversational capability.
* Cross-lingual context retention using a shared memory structure.
* Reuses previous intent for ambiguous follow-up messages.
* Lightweight architecture that is easy to understand and deploy.
* Fully extensible for advanced NLP and machine learning models.

## Future Enhancements

* VADER Sentiment Analysis
* TextBlob
* Hugging Face Transformers
* Rasa Framework
* Custom Machine Learning Classifiers
* Advanced Multilingual Language Models

## Author

**Danusree Devasenan**
