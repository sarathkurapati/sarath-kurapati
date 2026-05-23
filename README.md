### Hi, I'm Sarath 👋

**Associate AI Engineer @ MBK Solutions Pvt Ltd** · Hyderabad, India

I build ML systems for fintech and consumer products. I care about the boring parts that actually ship — clean data pipelines, models you can defend, and interfaces that don't make users think.

---

#### 🔭 What I'm working on

- **Stepping Stones** — Credit risk ML platform for collateral-backed subprime lending at MBK Solutions. LightGBM PD model (AUC 0.7374) trained on 1.33M LendingClub loans, served via FastAPI with real-time collateral, interest rate, and amortisation logic. Built with ECOA fair-lending compliance.


#### 📚 What I'm learning

- Agentic AI and multi-agent systems with LangGraph
- LLM fine-tuning with LoRA and Hugging Face
- Production system design for mobile-scale apps

---

#### 🧰 Tech I work with

**Languages**
`Python` · `SQL`

**Machine Learning**
`scikit-learn` · `TensorFlow` · `LightGBM` · `CNN` · `RNN` · `LSTM` · `Transfer Learning` · `MediaPipe`

**Generative AI & LLMs**
`LangChain` · `LangGraph` · `RAG` · `Prompt Engineering` · `LoRA` · `Hugging Face`
`OpenAI API` · `Azure OpenAI` · `Claude (Anthropic)` · `Gemini API` · `Llama 3.1`

**Vector DBs & Retrieval**
`Astra DB` · `Vector Embeddings` · `Similarity Search`

**Backend & APIs**
`FastAPI` · `Flask` · `REST APIs`

**Frontend & Apps**
`Flutter` · `Streamlit` · `HTML/CSS/JavaScript`

**Infrastructure & Tools**
`Docker` · `Git` · `MySQL` · `NGINX` · `Power BI`

---

#### 🛠️ Selected projects

#RepoSage — Code-Aware RAG System for Codebase Q&A
Stack: Python · FastAPI · tree-sitter · Qdrant · Voyage AI · Llama 3.3 70B · React
• Designed AST-based code chunking with tree-sitter across 5 languages, extracting complete function/class/method units with file path
and line-range metadata, eliminating the semantic fragmentation of fixed-size splitting.
• Built a full retrieval pipeline: GitHub clone → syntax-tree parsing → Voyage voyage-code-3 vector embeddings → Qdrant cosine
similarity search → Llama 3.3 70B answer generation with inline citations.
• Implemented atomic swap re-indexing with deterministic UUID5 point IDs derived from repo + file + line, enabling zero-downtime
re-ingestion and collision-free multi-repo isolation in a shared vector collection.
• Enforced answer grounding via a system prompt constraining the LLM to cite only retrieved chunks, with a configurable cosine
similarity threshold to suppress low-confidence retrievals.
• Shipped end-to-end: FastAPI REST backend (/ingest, /query) with async thread offloading and a React/Tailwind chat UI featuring
clickable citations that deep-link to GitHub source lines.
#Guardrailed Enterprise AI Assistant with LangGraph (Responsible AI Pipeline)
Stack: LangGraph · LangChain · OpenAI/Llama 3.1 · Presidio · FastAPI · Docker · Python
• Built a production-oriented LLM assistant using LangGraph to orchestrate a multi-stage pipeline with dedicated safety, validation, and
compliance nodes layered around the core generation step.
• Designed an input-guardrail node to detect and block prompt injection, PII leakage, and out-of-scope queries before they reach the
LLM, using a mix of regex, classifier checks, and LLM-based screening.
• Implemented an output-validation loop with LangGraph's cyclic graphs — responses pass through toxicity, bias, and hallucination
checks and are routed back for regeneration if they fail, reducing unsafe outputs.
• Added PII detection and redaction (Presidio) within the graph state so sensitive data is masked in both logs and responses, and a
citation/grounding check flagging ungrounded claims.
• Integrated human-in-the-loop escalation using LangGraph checkpoints, plus audit logging and decision traceability across every node
to support transparency and governance.

#### 🎯 What I'm interested in

ML for financial services · agentic AI and LLM applications · consumer mobile apps · clean system design

---

#### 📫 Reach me

- 📧 **Email:** [sarathkurapati@gmail.com](mailto:sarathkurapati@gmail.com)
- 💼 **LinkedIn:** [linkedin.com/in/sarath-kurapati](https://www.linkedin.com/in/sarath-kurapati/)
- 🐙 **GitHub:** you're already here

---

⭐ My pinned repos below show what I've actually built — feel free to dig in.
