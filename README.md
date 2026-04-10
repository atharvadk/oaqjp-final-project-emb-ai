# Final project
# AI-Based Emotion Detection Web Application

## 📌 Project Overview

This project is an AI-based web application that analyzes customer feedback and detects emotions expressed in text using IBM Watson NLP services.

The application processes user input and identifies the following emotions:

- Anger
- Disgust
- Fear
- Joy
- Sadness

It also determines the **dominant emotion**.

---

## 🎯 Objectives

- Build an emotion detection system using Watson NLP API
- Process and format API responses
- Package the application as a Python module
- Perform unit testing
- Deploy the application using Flask
- Implement error handling
- Ensure code quality using static analysis (Pylint)

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python 3 | Core language |
| Flask | Web framework |
| IBM Watson NLP API | Emotion analysis |
| Requests Library | HTTP communication |
| Pylint | Static code analysis |

---

## 📁 Project Structure

```
oaqjp-final-project-emb/
│
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
│
├── templates/
│   └── index.html
│
├── static/
│   └── mywebscript.js
│
├── server.py
├── test_emotion_detection.py
└── README.md
```

---

## 🚀 Features

### ✔ Emotion Detection

- Takes user input text
- Sends request to Watson NLP API
- Extracts emotion scores
- Identifies dominant emotion

### ✔ Output Format

```json
{
  "anger": score,
  "disgust": score,
  "fear": score,
  "joy": score,
  "sadness": score,
  "dominant_emotion": "emotion_name"
}
```

### ✔ Web Interface

- Built using Flask
- Accessible on `localhost:5000`
- Displays formatted emotion analysis

### ✔ Error Handling

Handles blank input and returns:

```
Invalid text! Please try again!
```

### ✔ Unit Testing

Test cases include:

| Test Input | Expected Dominant Emotion |
|---|---|
| "I am glad this happened" | Joy |
| "I am really mad about this" | Anger |
| "I feel disgusted" | Disgust |
| "I am so sad" | Sadness |
| "I am afraid" | Fear |

### ✔ Code Quality

- Static code analysis using Pylint
- Achieved **10/10 score**

---

## ⚙️ Setup Instructions

### 1. Clone Repository

```bash
git clone <your-repo-url>
cd oaqjp-final-project-emb
```

### 2. Install Dependencies

```bash
python3 -m pip install requests flask pylint
```

### 3. Run Application

```bash
python3 server.py
```

### 4. Access Application

Open in browser:

```
http://localhost:5000
```

---

## 🧪 Testing

Run unit tests:

```bash
python3 test_emotion_detection.py
```

Expected output:

```
All tests passed!
```

---

## 🌐 API Endpoint

```
/emotionDetector?textToAnalyze=your_text_here
```

**Example:**

```
http://127.0.0.1:5000/emotionDetector?textToAnalyze=I%20am%20happy
```

---

## ⚠️ Error Handling Example

**Input:** *(empty text)*

**Output:**

```
Invalid text! Please try again!
```

---

## 📊 Static Code Analysis

Run:

```bash
pylint server.py
```

Result:

```
Your code has been rated at 10.00/10
```

---

## 🎉 Conclusion

This project demonstrates:

- Integration of AI APIs
- Backend development with Flask
- Data processing and validation
- Software testing and quality assurance

---

## 👨‍💻 Author

**Atharva Kavade**

---

## 📄 License

This project is part of IBM Skills Network Labs and is licensed under [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0).
