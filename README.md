# Content-Checker App


## Overview

The **Content-Checker App** is a content moderation platform that analyzes and approves text posts and audio content. It uses advanced **Natural Language Processing (NLP)** techniques for sentiment analysis, harmful content detection, and integrates **speech-to-text conversion** to handle audio content. The platform aims to ensure that submitted content complies with community guidelines by flagging inappropriate or harmful content.

## Key Features

- **Text and Audio Content Moderation**  
  - Approves or flags text posts and audio content based on community guidelines.
  - Converts audio content to text using **Speech-to-Text APIs** (OpenAI Whisper or Google Speech-to-Text).
  
- **Natural Language Processing (NLP)**  
  - Implements sentiment analysis to assess the tone of the content.
  - Detects harmful content like aggressive behavior, suicidal ideation, and self-harm.
  
- **Dynamic User Interface**  
  - Built with **ReactJS, HTML, and CSS**, offering a responsive and user-friendly interface.
  
- **RESTful API Integration**  
  - Seamless integration with external APIs for speech-to-text conversion and sentiment analysis.
  
- **Moderation Logic**  
  - Allows moderators to approve, flag, or reject content based on predefined guidelines.
  
- **Scalability and Performance**  
  - Optimized backend and API calls for faster processing and higher scalability.

## Tech Stack

- **Frontend**:  
  - ReactJS  
  - HTML, CSS (Responsive Design)
  
- **Backend**:  
  - Node.js (Server-side processing and managing moderation decisions)

- **Speech-to-Text**:  
  - OpenAI Whisper or Google Speech-to-Text API

- **Natural Language Processing (NLP)**:  
  - Sentiment Analysis  
  - Harmful Content Detection (Aggression, Suicidal Ideation, Self-harm)

## Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (Backend development)
- **npm** or **yarn** (Package manager)
- **API Keys** for **OpenAI Whisper** or **Google Speech-to-Text** (for speech-to-text functionality)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/content-checker-app.git
Navigate into the project folder:

bash
Copy
Edit
cd content-checker-app
Install dependencies for both frontend and backend:

For the frontend (ReactJS):

bash
Copy
Edit
cd client
npm install
For the backend (Node.js):

bash
Copy
Edit
cd server
npm install
Set up API keys for speech-to-text and other services in the environment variables.

Running the App
Start the backend server:

bash
Copy
Edit
cd server
npm start
Start the React frontend:

bash
Copy
Edit
cd client
npm start
The app should now be running on http://localhost:3000.

Usage
Upload Audio/Text
Users can upload text posts or audio files for moderation.

Content Analysis

Audio files will be converted to text using the selected speech-to-text API.
Text will be analyzed for sentiment and harmful content using NLP models.
Moderation Panel
Moderators can view flagged content and approve or reject it based on the analysis results.

API Endpoints
/api/analyzeText
POST: Analyze text for sentiment and harmful content.
Request body: { "text": "Your text content here" }
Response: { "sentiment": "positive/negative/neutral", "flagged": true/false, "reason": "aggression/suicidal ideation" }
/api/analyzeAudio
POST: Convert audio to text and analyze it.
Request body: { "audioFile": "<file>" }
Response: { "transcription": "Transcribed text", "sentiment": "positive/negative/neutral", "flagged": true/false }
Contributing
Contributions are welcome! Please fork this repository and submit a pull request with your improvements.
