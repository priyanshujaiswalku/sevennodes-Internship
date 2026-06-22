# Sevennodes-Internship

# 📄 PDF-LLM Chatbot

A web-based application that allows users to upload PDF files, process their content, and interact with documents using an intelligent chatbot interface. The system supports text extraction, table processing, and optional summarization using DeepSeek R1.

---

## 🚀 Features

* 📂 **PDF Upload**
  Upload PDF files for processing and analysis.

* 🧾 **Text & Table Extraction**
  Extract textual content and structured tables using PyMuPDF and Camelot.

* 🤖 **Chat Interface**
  Ask questions based on extracted content through a conversational chatbot.

* 📝 **Optional Summarization**
  Summarize long documents using DeepSeek R1’s advanced reasoning capabilities.

---

## 📋 Prerequisites

Ensure the following are installed:

* Python (3.8 or higher)
* pip (Python package manager)
* Node.js & npm

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/pdf-chatbot.git
cd pdf-chatbot
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
```

### 3️⃣ Activate Virtual Environment

**Windows:**

```bash
venv\Scripts\activate
```

**Mac/Linux:**

```bash
source venv/bin/activate
```

### 4️⃣ Install Backend Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file in the root directory and configure:

### 1. Google Drive API

* Create a project in Google Cloud Console
* Enable Google Drive API
* Download the JSON credentials file
* Place it in the project root

---

### 2. DeepSeek API Key

Add the following in `.env`:

```env
DEEPSEEK_API_KEY=your-deepseek-api-key
```

---

## 💻 Frontend Setup

### Navigate to frontend folder

```bash
cd frontend
```

### Install dependencies

```bash
npm install
```

### Configure frontend environment

```env
NEXT_PUBLIC_BASE_URL=http://127.0.0.1:5000
```

---

## ▶️ Running the Application

### 1. Start Backend (Flask)

```bash
python app.py
```

Backend runs at:
👉 http://127.0.0.1:5000/

---

### 2. Start Frontend (Next.js)

```bash
npm run dev
```

---

## 🧪 Testing

### Test Google Drive Integration

```bash
python test_google_drive.py
```

### Test DeepSeek API

```bash
python test_r1.py
```

---

## 📁 Project Structure

```
pdf-chatbot/
│── app.py
│── templates/
│   └── index.html
│── utils/
│   ├── google_drive.py
│   └── api_utils.py
│── frontend/
│── test_google_drive.py
│── test_r1.py
```

---

## 🛠️ Key Libraries

* Flask – Backend web framework
* PyMuPDF – PDF text extraction
* Camelot – Table extraction
* Hugging Face Transformers – NLP pipeline
* Next.js – Frontend framework

---

## ⚠️ Known Limitations

* Summarization can be slow for large documents.
* Performance depends on system resources and API latency.

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 🤝 Contribution

Contributions are welcome!
Feel free to fork the repository and submit pull requests.

---

## ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub!

---
