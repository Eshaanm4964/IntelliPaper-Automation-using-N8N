ScholarFlow: Autonomous Academic Research & Synthesis PipelineScholarFlow is an enterprise-grade autonomous research pipeline that orchestrates Large Language Models (LLMs) and academic APIs to transform a single prompt into a structured, human-centric research paper. By leveraging n8n for workflow orchestration, it automates the entire lifecycle of academic writing—from literature retrieval to AI-detection mitigation.
🏗️ System ArchitectureThe pipeline follows a modular, linear progression with iterative loops for quality assurance:Code snippetgraph TD
    A[Webhook Trigger] --> B[Data Sanitization]
    B --> C[Research API Integration]
    C --> D[Synthesis & Theme Extraction]
    D --> E[Outline Generation]
    E --> F[Full-Text Synthesis]
    F --> G[Humanizer Engine]
    G --> H{AI Detection Check}
    H -- > 20% --> G
    H -- < 20% --> I[PDF Rendering]
    I --> J[Final Delivery]
🧠 Core Capabilities1. Intelligent Literature RetrievalUnlike standard LLMs, ScholarFlow ground its outputs in real-world data by querying Semantic Scholar and OpenAlex. It extracts metadata, abstracts, and key findings to ensure factual grounding.2. Thematic Synthesis & Gap AnalysisThe system doesn't just summarize; it analyzes. The Theme Analyzer node identifies:Prevailing methodological trends.Contradictions in current literature.Under-researched "gaps" for the paper to address.3. Advanced Linguistic Engineering (Humanization)To counter the "uniformity" of standard AI prose, the pipeline utilizes a recursive Detection Reduction Engine. It optimizes for:Burstiness: Varying sentence length and structural complexity.Perplexity: Utilizing nuanced vocabulary to mirror human academic styles.Iterative Refinement: Employs conditional logic to re-process text until it meets a sub-20% detection probability threshold.🛠️ Tech StackComponentTechnologyOrchestrationn8nReasoning EnginesOpenAI GPT-4o / Anthropic Claude 3.5 SonnetResearch DatabasesSemantic Scholar API / OpenAlexPDF Enginen8n Binary & HTML ConversionInterfaceRESTful Webhooks⚙️ Quick Start1. Clone & Environment SetupBashgit clone https://github.com/yourusername/scholarflow.git
cd scholarflow
2. Workflow ImportOpen your n8n instance.Select Import from File and upload the scholarflow_workflow.json located in the root directory.Configure your credentials for OpenAI (or your chosen LLM provider) and Semantic Scholar.3. Triggering the PipelineThe pipeline listens for a JSON payload via POST request:JSON{
  "topic": "The impact of quantum computing on modern cryptography"
}
📈 Performance TargetsWord Count: 1,500 – 2,500 words.Target AI Detection: $\le 20\%$.Format: IEEE/APA compliant structure (Abstract, Intro, Methods, Discussion, Refs).🔐 Ethical Disclaimer & LicenseScholarFlow is a tool designed for research assistance, drafting, and educational exploration. Users are responsible for ensuring academic integrity and adhering to the specific policies of their institutions regarding the use of AI in writing.Distributed under the MIT License. See LICENSE for more information.
