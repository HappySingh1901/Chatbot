---
"Image Recognition Chatbot"
---

# VisualTag Chatbot

This is a simple web-based chatbot with image recognition capabilities. It allows users to send text or image inputs and get meaningful responses using Google's Gemini 1.5 Flash API. Built with Flask and JavaScript, it’s lightweight and deployable on Vercel link (https://chatbot-3-theta.vercel.app/).

---

## Repository

GitHub Link: [https://github.com/Sandy-365/CHATBOT-3](https://github.com/Sandy-365/CHATBOT-3)

---

## Features

- Text and image chat interface  
- Image understanding and summarization  
- Google Gemini API integration  
- Simple HTML/CSS/JS frontend  
- Lightweight Flask backend  
- Vercel deployment ready

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Sandy-365/CHATBOT-3.git
cd CHATBOT-3
```

### 2. Install Requirements

```bash
pip install Flask google-generativeai Pillow
```

### 3. Set API Key

```bash
export API_KEY="your_google_generative_ai_key"
```

> On Windows:

```cmd
set API_KEY=your_google_generative_ai_key
```

### 4. Run the Application

```bash
python index.py
```

Visit `http://localhost:5000` in your browser.

---

## App Flow

1. Load the homepage and navigate to the chatbot.  
2. Enter a message or upload an image.  
3. Submit the form to receive a response from the Gemini API.  
4. View conversation history on the chat screen.

---

## Configuration for Vercel

Ensure your `vercel.json` is correctly set:

```json
{
  "version": 2,
  "builds": [
    {
      "src": "./index.py",
      "use": "@vercel/python",
      "config": {
        "runtime": "python3.8"
      }
    }
  ],
  "routes": [
    {
      "src": "/(.*)",
      "dest": "/"
    }
  ]
}
```

Add `API_KEY` in the environment settings in Vercel dashboard.

---

## Tech Stack

- Flask (Python)  
- HTML, CSS, JavaScript  
- Google Gemini 1.5 Flash  
- Pillow (Image processing)  
- Vercel (Hosting)

