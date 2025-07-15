# 🇮🇳 YojanaSaathi – Government Schemes Assistant

YojanaSaathi is a conversational AI assistant that helps Indian citizens understand and discover welfare schemes in Hindi, English, or Hinglish. It offers personalized responses to user queries based on a curated dataset of government scheme documents, powered by Google's Gemini API and a user-friendly Streamlit UI.

## 🌐 Live Demo
Deployed at: [https://yojanasaathi.streamlit.app](https://yojanasaathi.streamlit.app)  
Source Code: [https://github.com/codezaemon/yojanasaathi](https://github.com/codezaemon/yojanasaathi)

---

## 🧠 Sub-theme
**Building for Bharat** — Leveraging GenAI to bridge the awareness gap in rural and underserved communities about government schemes, ensuring inclusivity and access.

---

## 📦 Tech Stack

| Component             | Tool/Library                        | License  | Role/Use |
|----------------------|--------------------------------------|----------|----------|
| Frontend UI          | Streamlit v1.46.1                   | Apache 2.0 | Interactive chatbot interface |
| Language Model       | Google Gemini 1.5 Flash via API     | Proprietary | Natural language generation |
| Embeddings (Optional/Future) | SentenceTransformers (planned) | Apache 2.0 | For RAG integration |
| Styling              | Custom CSS with Inter font          | -        | WhatsApp-inspired dark UI |
| Environment Config   | python-dotenv                       | BSD-3     | Load Gemini API key |
| Deployment           | Streamlit Cloud                     | -         | Hosting the prototype |
| Document Storage     | Plaintext `.txt` files              | -         | Context for Gemini queries |

---

## 🚀 Features

- Conversational UI with WhatsApp-inspired styling
- Supports Hindi, English, and Hinglish queries
- Responds with clear, simplified answers based on official scheme details
- Context-driven prompting using `.txt` scheme files
- Hosted on Streamlit Cloud with no backend server needed

---

## 📁 Project Structure

```
yojanasaathi/
│
├── app.py                # Main Streamlit app
├── schemes/              # Folder containing .txt files for each scheme
├── requirements.txt      # Python dependencies
├── .env                  # GEMINI_API_KEY (not committed)
├── .gitignore           # Ignore venv, .env, etc.
└── README.md            # You're reading it!
```

---

## 🛠️ Setup Guide (Run Locally)

### 1. Clone the repository

```bash
git clone https://github.com/codezaemon/yojanasaathi.git
cd yojanasaathi
```

### 2. Create virtual environment

```bash
python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Setup Gemini API Key

Create a `.env` file in the root directory:

```ini
GEMINI_API_KEY=your_api_key_here
```

Get your API key from: https://makersuite.google.com/app/apikey

### 5. Run the app

```bash
streamlit run app.py
```

---

## 📄 Sample Schemes Included

- Ayushman Bharat (PM-JAY)
- PM KISAN
- Ujjwala Yojana
- NSAP (Old Age/Widow Pension)
- Post Matric Scholarship for Minorities
- Savitribai Phule Fellowship
- Swachh Bharat Mission – Urban

---

## 📝 Open Source Attribution

| Library | Version | License | Role | Link |
|---------|---------|---------|------|------|
| Streamlit | 1.46.1 | Apache 2.0 | Web UI | https://github.com/streamlit/streamlit |
| python-dotenv | 1.1.1 | BSD-3 | Load environment variables | https://github.com/theskumar/python-dotenv |
| google-generativeai | 0.8.5 | Apache 2.0 | Gemini model integration | https://github.com/google/generative-ai-python |
| pandas, requests, etc. | latest | Varies | Supporting utilities | PyPI |

---

## 💡 Future Enhancements

- Add FAISS + Embeddings for true RAG retrieval
- Multilingual voice support (speech-to-text)
- Scheme eligibility checker using form inputs
- Auto-indexing of new government schemes

---

## 🙏 Acknowledgements

- Google Gemini API
- Streamlit Cloud for deployment
- Government of India scheme portals for open data

---

## 💬 License

This repository is open for educational and non-commercial use under the MIT License.

