🚀 Overview

ScholarFlow is an end-to-end automated research paper generation pipeline built using n8n, Large Language Models (LLMs), and academic research APIs.

It streamlines the academic writing workflow by:

Accepting a research topic via Webhook

Fetching relevant research papers

Analyzing themes and trends

Generating a structured academic paper

Reducing AI-detection signals

Estimating AI detection probability

Delivering a downloadable PDF output

This project demonstrates intelligent automation, AI orchestration, and workflow engineering in a production-ready pipeline.

🏗️ System Architecture
Webhook
   ↓
Input Cleaning
   ↓
Research API (Semantic Scholar / OpenAlex)
   ↓
Extract & Summarize Papers
   ↓
AI – Theme Analyzer
   ↓
AI – Research Outline Generator
   ↓
AI – Full Paper Writer
   ↓
AI – Humanizer (AI Detection Reduction)
   ↓
AI – AI Detection Estimator
   ↓
Conditional Logic (≤20% Target)
   ↓
Convert to PDF
   ↓
Respond to Webhook

🧠 Core Features
🔎 1. Automated Research Retrieval

Fetches relevant academic papers via research APIs

Extracts abstracts, titles, authors, and metadata

Supports scalable academic search

📊 2. AI-Based Thematic Analysis

Identifies research trends

Detects methodological patterns

Highlights research gaps

Synthesizes key debates

📝 3. Structured Research Paper Generation

Automatically generates:

Title

Abstract

Introduction

Literature Review

Methodology

Results & Discussion

Conclusion

Maintains academic tone and logical structure.

🧬 4. AI-Detection Reduction Engine

Implements advanced rewriting techniques to:

Increase burstiness (sentence variation)

Reduce uniform syntactic patterns

Remove repetitive academic phrasing

Introduce natural stylistic variation

Target ≤20% estimated AI-detection probability

📈 5. AI Detection Estimation

Evaluates probability of AI-generated classification

Uses conditional logic for iterative rewriting

Ensures content refinement before final export

📄 6. Automated PDF Generation

Converts final output into downloadable PDF

Delivered via Webhook response

Supports API-based integration

🛠️ Technology Stack
Component	Technology
Workflow Automation	n8n
Language Model	OpenAI / Compatible LLM
Research Data	Semantic Scholar / OpenAlex
API Testing	Postman
File Conversion	n8n Binary Conversion
Output Format	PDF / TXT
⚙️ Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/yourusername/scholarflow.git
cd scholarflow

2️⃣ Import Workflow into n8n

Open your n8n instance

Import the provided workflow JSON

Configure node credentials

3️⃣ Configure API Credentials

Set up:

LLM API Key

Research API Key (optional for higher rate limits)

4️⃣ Trigger the Workflow

Send a POST request to the production webhook:

{
  "topic": "Artificial Intelligence in Healthcare"
}

📦 Example Output

1500–2000 word structured research paper

AI detection probability estimate

Downloadable PDF file

Clean academic formatting

🎯 Use Cases

Academic draft generation

Research ideation

Literature exploration

AI workflow experimentation

Automation portfolio demonstration

🔐 Disclaimer

This project is intended for:

Research assistance

Draft generation

Educational experimentation

Users are responsible for:

Verifying originality

Adding proper citations

Ensuring academic integrity

Complying with institutional policies

🔮 Future Enhancements

Automatic citation formatting (APA/MLA/Chicago)

DOI-based reference auto-generation

Real plagiarism API integration

Frontend dashboard interface

Multi-language research support

Deployment-ready API wrapper

🤝 Contributing

Contributions are welcome.

Fork the repository

Create a new feature branch

Submit a pull request

For major improvements, please open an issue first.

📜 License

This project is licensed under the MIT License.
