# 🤖 AI-Driven Development 30-Day Challenge – Task 4
*Assignment Type:* Practical Project
*Marks:* 10
*Deadline:* 48 Hours
*Class Slot:* Friday 6:00 PM to 9:00 PM

---

## 📌 Task 4: Context7 MCP Server Integration & AI Study Agent Development

### 1. What Are MCP Servers?

MCP (Model Context Protocol) servers act as bridges between your AI model or CLI and the tools you want to use. They provide controlled access to:

- Files
- Local functions
- External systems like Github, Firebase, etc.

In simple terms, MCP servers give Gemini CLI the *"tools"* to perform real actions, beyond just replying with text.

---

### 2. Why MCP Servers Are Useful?

- Instantly add new abilities to AI models.
- Follow a standard format for easy integration across systems.
- Remove manual wiring of every tool, simplifying setup.
- Make your AI setup modular and maintainable.
- Allow students to build agents without deep backend coding.

---

### 3. The Problem with Gemini CLI

- Gemini CLI alone cannot create full agents.
- Lacks strong agent-building support, causing frustration and limitations.

---

### 4. The Solution: Context7 MCP Server

- [Context7](https://context7.com) is a *complete MCP server* exposing powerful tools and auto-updating documentation.
- Supports Python, OpenAgents SDK, Supabase, FastAPI, and other modern frameworks.
- Keeps Gemini CLI agent-building error-free and up to date.
- Eliminates the hassle of checking multiple documentation sources.

---

### 5. Task Objective: Connecting Context7 MCP Server to Gemini CLI

- Follow the [MCP Server Setup Guide](https://www.notion.so/Personalization-Chatbot-with-Chainla-26764465197680728913d:57ee7d1803) to connect Context7 MCP Server with Gemini CLI.
- This connection enables your AI agent to access powerful tools needed for the next practical task.

---

### 6. Practical Task: Build the Study Notes Summarizer & Quiz Generator Agent

Using *OpenAgents SDK, **Streamlit, **PyPDF, **Context7 MCP, and **Gemini CLI*, create an agent that:

- *PDF Summarizer:*
  - User uploads a PDF.
  - Text is extracted using PyPDF.
  - Agent generates a clean, meaningful summary with customizable UI display.

- *Quiz Generator:*
  - After summarization, user clicks *Create Quiz*.
  - Agent reads the original PDF and generates multiple-choice or mixed-style quizzes.

---

### 7. Deliverables

- Fully deployed Study Notes Summarizer & Quiz Generator agent.
- GitHub repository with source code and README.
- Screenshot of Gemini CLI prompt used during agent creation.
- Evidence of successful MCP server connection.

![MCP Server Connected](mcp.png)

---

### 8. Important Links

- Context7 Website: [https://context7.com](https://context7.com)
- MCP Server Setup Guide: [Notion Guide](https://www.notion.so/Personalization-Chatbot-with-Chainla-26764465197680728913d:57ee7d1803)

---

# 📚 Professional AI Study Agent

![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-1.32+-FF4B4B.svg)
![Gemini](https://img.shields.io/badge/AI-Gemini%202.0%20Flash-8E75B2.svg)

An advanced, AI-powered research assistant designed to transform static PDF documents into interactive learning experiences. Built with **Google Gemini 2.0 Flash**, this agent automatically generates summaries, quizzes, concept maps, and structured study notes to help you master any material faster.

## 🚀 Features

- **📄 Smart Executive Summaries**: Instantly get the gist of long research papers or textbooks.
- **🧠 Interactive Knowledge Graphs**: Visualize complex relationships between topics using AI-generated Mermaid.js diagrams.
- **📝 Infinite Auto-Quizzing**:
    - Test your knowledge with AI-generated multiple-choice questions.
    - **Dynamic Generation**: Click "Generate More Questions" to create endless practice sets.
    - Immediate feedback with detailed explanations.
- **📓 AI Structured Study Notes**: Automatically extracts:
    - Key Definitions
    - Core Concepts
    - Important Facts/Dates
    - Formulas & Rules
- **✍️ Personal Note-Taking**: Add your own insights alongside the AI-generated content.
- **🎨 Professional UI**: A modern, clean interface with pill-shaped navigation, gradient aesthetics, and a user-friendly experience.
- **💾 Session Memory**: Keeps track of your current study session context.

## 🛠️ Tech Stack

- **Frontend**: Streamlit (Python)
- **AI Engine**: Google Gemini 2.0 Flash (via `google-generativeai`)
- **PDF Processing**: PyPDF2
- **Visualization**: Mermaid.js (rendered via Streamlit)
- **Environment**: Python Dotenv

## ⚙️ Installation & Setup

1. **Clone the Repository**
   ```bash
   git clone <repository-url>
   cd Task-4
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure API Key**
   Create a `.env` file in the root directory and add your Google Gemini API key:
   ```env
   GEMINI_API_KEY=your_actual_api_key_here
   ```

4. **Run the Application**
   ```bash
   streamlit run summarizer_quiz_agent/app.py
   ```

## 📂 Project Structure

```
Task-4/
├── .env                     # API Keys (Ignored by Git)
├── requirements.txt         # Python Dependencies
├── summarizer_quiz_agent/   # Main Application Source
│   ├── app.py               # Main Streamlit Entry Point
│   ├── summarizer.py        # AI Summary Logic
│   ├── quiz_generator.py    # AI Quiz Logic
│   ├── notes_generator.py   # AI Study Notes Logic
│   ├── concept_map.py       # AI Graph Logic
│   ├── pdf_utils.py         # PDF Parsing
│   ├── memory.py            # Session State Management
│   └── utils.py             # API & Helper Functions
└── README.md                # Documentation
```

## 👤 Creator

**Muhammad Sufiyan**  
*Created with ❤️ using Python & Generative AI.*