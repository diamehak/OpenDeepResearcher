# 🚀 OpenDeepResearcher

OpenDeepResearcher is an AI-powered multi-agent research assistant that autonomously plans, searches, analyzes, and synthesizes information into structured reports. The system uses locally hosted large language models via LM Studio, enabling private, cost-efficient, and intelligent deep research workflows without relying on cloud LLM APIs.

---

## ✨ Features

- 🔍 Autonomous research planning with subquestion generation
- 🌐 Real-time web search using Tavily API
- 🧠 Multi-agent reasoning pipeline (Planner → Searcher → Writer)
- 📝 Academic-style report generation with citations
- 🔒 Local LLM inference using LM Studio (privacy-friendly)
- 📊 Structured JSON research plans
- ⚡ Modular and extensible architecture

---

## 🏗️ System Architecture

The system follows an agent-based pipeline:

1. **Planner Agent**
   - Breaks user queries into 6–8 focused subquestions
   - Generates structured research plans
   - Extracts constraints and keywords

2. **Searcher Agent**
   - Retrieves relevant sources using Tavily API
   - Collects titles, URLs, snippets, and relevance scores

3. **Writer Agent**
   - Synthesizes findings into a comprehensive academic report
   - Adds citations and references
   - Saves final output to file

---

## 🤖 Model & Runtime

**LLM Runtime:** LM Studio  
**Model:** Qwen 2.5 7B Instruct  
**Inference:** Local (offline capable)

Benefits:

- No cloud dependency
- Improved privacy
- Lower cost
- Full control over model execution

---

## 📂 Project Structure

```
OpenDeepResearcher/
│── agents/
│     ├── planner_agent.py
│     ├── searcher_agent.py
│     └── writer_agent.py
│
│── main.py
│── requirements.txt
│── README.md
│── LICENSE
│── .gitignore
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/diamehak/OpenDeepResearcher.git
cd OpenDeepResearcher
```

Create virtual environment:

```bash
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 🧠 LM Studio Setup

1. Install **LM Studio**
2. Download **Qwen 2.5 7B Instruct** model
3. Start the LM Studio local server
4. Ensure API endpoint is running:

```
http://127.0.0.1:1234
```

---

## 🔑 Environment Variables

Create a `.env` file in the project root:

```
TAVILY_API_KEY=your_api_key_here
```

---

## ▶️ Usage

Run the main program:

```bash
python main.py
```

Enter your research question when prompted.

Example:

```
Impact of artificial intelligence on healthcare diagnostics
```

The system will:

1. Generate subquestions
2. Search for sources
3. Produce a structured research report
4. Save output to a file

---

## 📊 Example Output

The system generates:

- Research plan JSON file
- Detailed terminal logs
- Final academic report (.txt)

---

## 🎯 Use Cases

- Academic research assistance
- Literature reviews
- Market analysis
- Technical research
- Policy research
- Automated report generation

---

## 🔮 Future Improvements

- Memory-enabled agents
- Multi-modal document ingestion (PDFs)
- Citation formatting (APA/IEEE)
- Web UI dashboard
- Vector database integration
- Streaming responses

---

## 🛠️ Tech Stack

- Python
- LM Studio
- Qwen 2.5 7B
- Tavily Search API
- Requests
- Agentic AI architecture

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch
3. Commit changes
4. Open a Pull Request

---

## 📜 License

This project is licensed under the MIT License.

---

## 👤 Author

Dia Mehak
AI / ML Developer | Agentic AI Enthusiast  

---

⭐ If you find this project useful, please consider giving it a star!
