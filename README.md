# 💬 LangChain Chatbot with Gemini + Gradio  
A simple, fast, and clean conversational AI chatbot powered by **Google Gemini (via LangChain)** and built using **Gradio** for a sleek web interface.

---

## 🚀 Features

- ⚡ Powered by **Gemini 2.0 Flash Lite** (via LangChain)
- 🧠 Conversational context memory
- 🎯 Always gives **one-line concise responses**
- 🌐 Web-based interface using **Gradio**
- 🧪 Easily extensible and experiment-friendly

---

## 📁 Project Structure

```bash
.
├── main.py                         # Main script with chatbot logic
├── requirements.txt               # Python dependencies
├── .env                           # Environment variables (API key, etc.)
└── README.md                      # Project documentation (you’re here)
```

---

## ⚙️ Requirements

Make sure you have the following before running:

- Python 3.9+
- Google Colab (optional but recommended for beginners)
- Google Gemini API key (set in `.env` file)
- Internet connection

---

## 🛠️ Installation & Setup

### 🔗 Step 1: Mount Google Drive in Colab

```python
from google.colab import drive
drive.mount('/content/drive')
```

### 📦 Step 2: Install Dependencies

```bash
!pip install gradio
!pip install -r "/content/drive/MyDrive/Langchain/Projects/Project 1/requirements.txt"
```

### 🔐 Step 3: Create a `.env` File

Place it in:

```
/content/drive/MyDrive/Langchain/Projects/Project 1/.env
```

Add your Gemini API key:

```env
GOOGLE_API_KEY=your_gemini_api_key_here
```

---

## 🧠 How It Works

- Initializes a Gemini model using `langchain_google_genai`
- Uses a persistent `chat_history` to hold memory of the conversation
- Sends messages as `SystemMessage`, `HumanMessage`, or `AIMessage`
- Parses and returns concise AI responses
- Gradio renders a simple chat interface with reset and send buttons

---

## 💡 Example Usage

- **Ask Anything**: “What's the capital of Italy?”
- **Instant, Smart Reply**: “Rome.”

---

## 🧽 Resetting Chat

Click the “Reset Chat” button in the Gradio UI to clear chat history and start fresh.

---

## 🛡️ Security Note

**NEVER** commit your `.env` file or expose your API keys publicly.  
Use `.gitignore` to prevent accidental leaks:

```
.env
```

---

## 🌟 Future Improvements

- Add speech-to-text / TTS
- Integrate other models like GPT-4 or Claude
- Make it multi-turn or task-aware
- Deploy on Hugging Face Spaces or Streamlit Cloud

---

## 🙌 Acknowledgments

- [LangChain](https://github.com/langchain-ai/langchain)
- [Google Generative AI](https://ai.google.dev/)
- [Gradio](https://www.gradio.app/)
- [OpenAI](https://openai.com/) (for inspiration)

