
## AI-Powered Academic Research Automation Engine

> An end-to-end research paper generation pipeline built with n8n, LLMs, and academic research APIs.

---

## 📌 Overview

ScholarFlow is an automated academic research pipeline that:

- Retrieves scholarly articles via research APIs  
- Performs AI-driven thematic analysis  
- Generates a structured academic research paper  
- Reduces AI-detection signals (target ≤20%)  
- Delivers downloadable PDF or TXT output  

This project demonstrates advanced workflow automation, API orchestration, and applied AI engineering.

---

## 🧠 Key Features

### 🔎 Automated Research Retrieval
- Integration with Semantic Scholar / OpenAlex APIs  
- Extracts abstracts, titles, authors, and metadata  
- Structured JSON parsing  

### 📊 AI-Based Thematic Analysis
- Identifies trends and research gaps  
- Synthesizes key debates  
- Extracts methodological patterns  

### 📝 Structured Research Paper Generation
Automatically generates:

- Title  
- Abstract  
- Introduction  
- Literature Review  
- Methodology  
- Results & Discussion  
- Conclusion  

### 🧬 AI Detection Reduction Engine
- Enhances sentence variation  
- Reduces repetitive AI phrasing  
- Improves burstiness and natural tone  
- Targets ≤20% estimated AI-detection probability  

### 📄 Automated File Export
- Converts output to PDF or TXT  
- Returns downloadable file via webhook  

---

## 🏗️ System Architecture

Webhook  
→ Input Cleaning  
→ Research API  
→ Extract & Summarize  
→ AI Theme Analyzer  
→ AI Outline Generator  
→ AI Full Paper Writer  
→ AI Humanizer  
→ AI Score Estimator  
→ Conditional Logic  
→ Convert to File  
→ Respond to User  

---

## 🛠️ Tech Stack

- **Workflow Automation:** n8n  
- **Language Model:** OpenAI / Compatible LLM  
- **Research Data:** Semantic Scholar / OpenAlex  
- **API Testing:** Postman  
- **File Conversion:** n8n Binary Nodes  

---

## ⚙️ Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/scholarflow.git
cd scholarflow
```

2. Import the workflow JSON into n8n.
3. Configure API credentials.
4. Activate the workflow.

---

## 📡 Usage

Send a POST request to the webhook:

```json
{
  "topic": "Artificial Intelligence in Healthcare"
}
```

The workflow will return a generated research paper file.

---

## 🔮 Future Enhancements

- Automatic citation formatting (APA/MLA/Chicago)  
- DOI-based reference extraction  
- Real plagiarism detection integration  
- Web dashboard frontend  
- Multi-language support  

---

## 🤝 Contributing

Pull requests are welcome.  
For major changes, please open an issue first.

---

## 📜 License

MIT License
