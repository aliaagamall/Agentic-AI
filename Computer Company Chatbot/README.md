# Computer Kabani Smart Chat Bot

## Overview

This project implements an AI-powered chatbot for a computer hardware company specializing in CPUs and GPUs. The chatbot acts as a virtual sales agent, providing product information, prices, and specifications from a Google Sheet. It also handles purchase requests by collecting customer details and sending notifications via email. This is based on a tutorial video, but adapted to use the Gemini API instead of OpenAI.

The chatbot supports natural language conversations, remembers context from previous messages, and automates responses 24/7 without human intervention.

<img width="1236" height="637" alt="image" src="https://github.com/user-attachments/assets/f26cb3cc-590c-4d9a-b8c2-95c3bc9a631b" />


## Features

- Responds to customer inquiries about product prices, specifications, and availability.
- Fetches real-time data from a Google Sheet (e.g., product models, manufacturers, categories, prices).
- Handles purchase intents by requesting customer name and phone number.
- Sends email notifications to the company owner with customer details and requested products.
- Maintains conversation history for contextual responses.
- Supports rule-based, retrieval-based, and AI-driven response generation.

## Technologies Used

- **AI Model**: Gemini API (for natural language understanding and generation).
- **Data Storage**: Google Sheets (for product inventory and details).
- **Email Integration**: Gmail API (for sending purchase notifications).
- **Memory**: In-memory storage for conversation history (configurable to retain up to 50 messages).
- **Programming Language**: Python (or specify if different).
- **Libraries**: google-api-python-client (for Google Sheets and Gmail), google-generativeai (for Gemini), and any other dependencies like langchain for agent orchestration if used.

## Prerequisites

- A Google account for Google Sheets and Gmail API access.
- Gemini API key (obtain from Google AI Studio).
- Google Cloud Project with Sheets and Gmail APIs enabled.
- OAuth credentials for Google APIs (download as JSON).

## Configuration

- **Model**: Configured to use Gemini (e.g., gemini-1.5-pro). Adjust in `agent.py` if needed.
- **Memory**: Retains up to 50 messages; modify in the memory setup.
- **System Prompt**: Defined in the agent to instruct the model on using tools and handling purchases.
