# 🤖 CodeMentor Chatbot

A friendly AI-powered programming tutor chatbot built with **Gradio** and **GROQ API**. CodeMentor helps beginners learn programming concepts with clear explanations and practical examples.

## ✨ Features

- **Interactive Chat Interface** - User-friendly Gradio web interface for real-time conversations
- **Programming Tutor** - Specialized in explaining Python, C++, and algorithms for beginners
- **Adjustable Creativity** - Control response creativity with a temperature slider (0.2 - 1.0)
- **Smart Error Handling** - Comprehensive error management with user-friendly messages
- **Chat History** - Maintains conversation context throughout the session
- **Clear Chat** - One-click button to reset chat history
- **Fast Responses** - Powered by GROQ's high-performance LLMs (llama-3.1-8b-instant)

## 🛠️ Technology Stack

- **Python** - Core programming language
- **Gradio** - Web UI framework for machine learning models
- **GROQ API** - Fast inference engine for LLMs
- **Requests** - HTTP client for API communication

## 📋 Prerequisites

Before you begin, make sure you have:

- **Python 3.8+** installed
- **GROQ API Key** (get one free from [console.groq.com](https://console.groq.com))
- **Internet connection** to reach GROQ API

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/musabtahirhub/codementor-chatbot.git
cd codementor-chatbot
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

Or manually install the required packages:

```bash
pip install gradio requests
```

### 3. Configure GROQ API Key

#### On Windows:
```bash
set GROQ_API_KEY=your_api_key_here
python app.py
```

#### On Linux/macOS:
```bash
export GROQ_API_KEY=your_api_key_here
python app.py
```

#### Alternative: Create a `.env` File

Create a `.env` file in the project root:

```
GROQ_API_KEY=your_api_key_here
```

Then run:
```bash
python app.py
```

### 4. Run the Application

```bash
python app.py
```

The chatbot will launch and typically be available at: `http://127.0.0.1:7860/`

## 📖 Usage

1. **Ask Questions** - Type your programming questions in the text box
2. **Adjust Creativity** - Use the slider to control how creative the responses should be:
   - **Lower values (0.2)** - More focused, factual responses
   - **Higher values (1.0)** - More creative, varied responses
3. **Clear Chat** - Click the "Clear Chat" button to start a new conversation
4. **Wait for Response** - The bot will generate a response using GROQ's AI model

### Example Questions

- "How do I write a Python function?"
- "Explain what recursion is"
- "How do I debug C++ code?"
- "What are algorithms?"

## ⚙️ Configuration

### Model Settings

Edit `app.py` to customize:

- **Model**: Change `MODEL_NAME` to use different GROQ models
  - Available: `llama-3.1-8b-instant`, `mixtral-8x7b-32768`, etc.
- **System Prompt**: Modify `SYSTEM_PROMPT` to change the chatbot's personality and expertise
- **Temperature Range**: Adjust the slider range in the UI
- **Timeout**: Change the request timeout (currently 30 seconds)

```python
MODEL_NAME = "llama-3.1-8b-instant"  # Change model here
SYSTEM_PROMPT = """Your custom instructions..."""  # Customize behavior
```

## 📁 Project Structure

```
codementor-chatbot/
├── app.py                 # Main application file
├── requirements.txt       # Python dependencies
├── README.md             # This file
└── .gitattributes        # Git LFS configuration
```

## 🔧 Error Handling

The chatbot includes comprehensive error messages:

- **🔑 Authentication Error** - Invalid or missing GROQ API key
- **⏳ Rate Limit** - Too many requests; wait before retrying
- **🔧 Server Error** - GROQ service temporarily unavailable
- **⏱️ Timeout** - Request took too long; try again
- **🌐 Connection Error** - Check your internet connection
- **❌ API Error** - Other API-related issues

## 📦 Dependencies

- `gradio>=3.0.0` - Web interface framework
- `requests>=2.28.0` - HTTP requests library

## 🤝 Contributing

Contributions are welcome! Feel free to:

- Report bugs
- Suggest new features
- Improve documentation
- Submit pull requests

## 📝 License

This project is open source and available under the MIT License. See LICENSE file for details.

## 🔗 Resources

- [GROQ Console](https://console.groq.com) - Get your API key
- [GROQ Documentation](https://console.groq.com/docs) - API reference
- [Gradio Documentation](https://www.gradio.app/docs) - UI framework docs
- [GROQ Models](https://console.groq.com/keys) - Available models list

## 💡 Tips for Best Results

1. **Ask Specific Questions** - More specific questions yield better answers
2. **Keep History Short** - Long conversations may slow down responses
3. **Use Clear Language** - Write clearly for better explanations
4. **Adjust Creativity** - Lower values for tutorials, higher for exploration
5. **Check API Quota** - Monitor your GROQ API usage on the console

## 🐛 Troubleshooting

### "API key not configured"
- Ensure `GROQ_API_KEY` environment variable is set correctly
- Restart the application after setting the key

### "Rate limit exceeded"
- Wait a few moments before sending another message
- Check your GROQ API usage limits

### "Connection error"
- Verify your internet connection
- Check if GROQ API is accessible from your network

### "Slow responses"
- Check your internet speed
- Verify GROQ API status
- Try a lighter model or lower temperature

## 📞 Support

For issues, questions, or feedback:

- Open an issue on [GitHub Issues](https://github.com/musabtahirhub/codementor-chatbot/issues)
- Check existing issues for solutions
- Provide detailed error messages and steps to reproduce

## 🎯 Roadmap

Potential future improvements:

- [ ] Support for multiple AI models
- [ ] Conversation history saving
- [ ] Code syntax highlighting
- [ ] Multiple language support
- [ ] Docker containerization
- [ ] Web deployment (Hugging Face Spaces, Replit, etc.)

---

**Made with ❤️ by [musabtahirhub](https://github.com/musabtahirhub)**

Star ⭐ this repo if you find it helpful!
