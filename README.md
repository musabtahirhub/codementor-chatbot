# 🤖 CodeMentor Chatbot

An AI-powered programming tutor chatbot built with **Gradio** and **GROQ API**. Learn Python, C++, and algorithms with friendly explanations and examples.

## ✨ Features

- Interactive chat interface with Gradio
- Programming tutor for beginners
- Adjustable response creativity (temperature slider)
- Smart error handling
- Chat history & clear button
- Fast responses powered by GROQ LLMs

## 🛠️ Tech Stack

- Python 3.8+
- Gradio (Web UI)
- GROQ API (Fast LLM inference)
- Requests (HTTP client)

## 🚀 Quick Start

### 1. Clone & Install
```bash
git clone https://github.com/musabtahirhub/codementor-chatbot.git
cd codementor-chatbot
pip install gradio requests
```

### 2. Set API Key

**Windows:**
```bash
set GROQ_API_KEY=your_api_key_here
```

**Linux/macOS:**
```bash
export GROQ_API_KEY=your_api_key_here
```

Get your free API key from [console.groq.com](https://console.groq.com)

### 3. Run
```bash
python app.py
```

Visit `http://127.0.0.1:7860/` in your browser.

## 📖 Usage

1. Type your programming question
2. Adjust creativity with the temperature slider
3. Click "Clear Chat" to start over
4. Get instant AI-powered explanations

### Example Questions
- "How do I write a Python function?"
- "Explain recursion"
- "How do I debug C++ code?"

## ⚙️ Configuration

Edit `app.py` to customize:
```python
MODEL_NAME = "llama-3.1-8b-instant"  # Change model
SYSTEM_PROMPT = """..."""  # Customize behavior
```

## 🐛 Troubleshooting

| Issue | Solution |
|-------|----------|
| API key not configured | Set `GROQ_API_KEY` environment variable |
| Rate limit exceeded | Wait a moment and retry |
| Connection error | Check your internet connection |
| Slow responses | Verify GROQ API status |

## 📝 License

MIT License - see LICENSE file

## 🔗 Resources

- [GROQ Console](https://console.groq.com)
- [Gradio Docs](https://www.gradio.app/docs)

---

**Made with ❤️ by [musabtahirhub](https://github.com/musabtahirhub)**

Star ⭐ this repo if helpful!
