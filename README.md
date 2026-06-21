# Culinary AI Bot

## Overview

Culinary AI Bot is a Python-based conversational assistant that provides recipe suggestions, manages conversation history, performs sentiment analysis on user input, and generates basic data visualizations.

The project demonstrates modular software design, object-oriented programming, file persistence, and simple natural language processing techniques.

---

## Features

### Recipe Recommendation System

The bot suggests recipes based on user input categories such as:

* Sweet
* Savory
* Healthy
* Quick meals

The recommendation engine is currently implemented as a mock AI service with predefined datasets, designed to be easily replaceable with a real API integration.

---

### Conversation History Management

All interactions between the user and the bot are stored locally in a JSON file.

Each record contains:

* Timestamp
* User input
* Bot response
* Detected sentiment

This allows persistent tracking of conversations across sessions.

---

### Sentiment Analysis

A lightweight sentiment analysis module classifies user messages into:

* Positive
* Negative
* Neutral

The classification is based on keyword matching and is intended as a simple demonstration of NLP logic rather than a production-grade model.

---

### Data Visualization

The system generates visual reports using Matplotlib:

1. Sentiment Distribution Graph
   Displays the frequency of positive, negative, and neutral interactions.

2. Service Quality Trend Graph
   Tracks a computed quality score over time based on sentiment shifts.

---

## Architecture

The project is structured into independent components:

* CulinaryBot: Main application controller
* AIService: Recipe generation logic (mock AI layer)
* HistoryManager: Handles loading and saving conversation history
* SentimentAnalyzer: Performs text sentiment classification
* Visualization: Generates analytical charts

This separation of concerns improves maintainability and scalability.

---

## Technologies Used

* Python 3.x
* JSON (data storage)
* Matplotlib (data visualization)
* Object-Oriented Programming (OOP)
* Exception handling

---

## Project Structure

```
AI-Food-Service-Bot/
│
├── culinary_bot.py
├── history.json
├── README.md
└── requirements.txt
```

---

## Installation

Clone the repository:

```
git clone <repository-url>
```

Navigate to the project directory:

```
cd AI-Food-Service-Bot
```

Install dependencies:

```
pip install matplotlib
```

---

## Usage

Run the application:

```
python culinary_bot.py
```

Example interaction:

```
You: I want something healthy
Bot: Quinoa salad with fresh vegetables
```

To exit the program:

```
exit
```

---

## Future Improvements

* Integration with real AI/LLM APIs
* Database support instead of JSON storage
* Web interface (Flask / FastAPI / React)
* Improved NLP-based sentiment analysis
* User authentication system
* Deployment to cloud environment

---

## Purpose of the Project

This project was built as a learning exercise to demonstrate:

* Software design principles
* Modular architecture
* Basic AI simulation concepts
* Data persistence techniques
* Simple data visualization workflows
