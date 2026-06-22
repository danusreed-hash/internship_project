# Multilingual Context-Aware Chatbot

## Overview

This project is a multilingual AI-powered chatbot designed to understand and respond in multiple languages, including English, Hindi, Spanish, and French. It supports context-aware conversations by maintaining session-based memory, enabling seamless follow-up interactions across different languages.

## Features

* Automatic language detection for English, Hindi, Spanish, and French.
* Multilingual conversation support with language switching during a session.
* Intent recognition for greetings, ticket booking, weather inquiries, status checks, cancellations, and expressions of gratitude.
* Session-based context memory for maintaining conversation continuity.
* Entity extraction for destination, date, time, and travel-related information.
* Interactive browser-based chat interface displaying language, intent, confidence score, and conversation turns.
* Lightweight Python backend using only standard library modules.
* Optional OpenRouter API integration for enhanced multilingual reasoning and response generation.

## Technologies Used

* Python
* HTML
* CSS
* JavaScript
* OpenRouter API
* Standard Python Libraries

## How to Run

Navigate to the project directory:

```bash id="f9y7mk"
cd multilingual_chatbot
```

Run the application:

```bash id="6b8r1s"
python app.py
```

Open the application in your browser:

```text
http://127.0.0.1:8000
```

## OpenRouter Online Mode

### Option 1: Enter API Key Through the Application

1. Start the application.
2. Open `http://127.0.0.1:8000`.
3. Enter your OpenRouter API key in the provided section.
4. Keep the model as `openrouter/auto` or specify another OpenRouter model.
5. Save the API key.

### Option 2: Configure Using Environment Variables

```env id="c6j3xq"
OPENROUTER_API_KEY=your-api-key
OPENROUTER_MODEL=openrouter/auto
```

Restart the application:

```bash id="7v2p1m"
python app.py
```

The chatbot will use OpenRouter's chat completion API for generating responses. If the API is unavailable or configuration is incorrect, the system automatically switches to offline rule-based responses.

## Example Conversation

**User:** Hello, I want to book a train ticket

**Bot:** I understood that you want to book a ticket. Please tell me the destination, date, and time.

**User:** मुझे दिल्ली जाना है

**Bot:** मैं समझ गया कि आप टिकट बुक करना चाहते हैं। कृपया date और time बताइए।

**User:** tomorrow evening

**Bot:** Got it. I will look for a train ticket to Delhi for tomorrow evening.

## System Workflow

```text
User Message
      ↓
Language Detection
      ↓
Intent Detection
      ↓
Entity Extraction
      ↓
Conversation State Update
      ↓
Response Generation
```

## Conversation Memory Stores

* Preferred language
* Previous intent
* Extracted entities (destination, date, time, travel mode)
* Complete conversation history

## Key Highlights

* Supports cross-lingual conversational continuity.
* Maintains context across multiple languages.
* Handles mixed-language messages through script detection and keyword matching.
* Easily extensible with advanced NLP frameworks and multilingual language models.

## Future Enhancements

* fastText for language identification
* Sentence Transformers for semantic understanding
* Rasa for conversational AI workflows
* MarianMT for machine translation
* mBART and NLLB for multilingual generation

## Author

**Danusree Devasenan**

