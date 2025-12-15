
---

# Questions 

---

### **Q1 - (open_ended_theory_question)**

Define the business problem this codebase solves in a domain of your choice (e.g., CPG, Manufacturing, Retail, Pharma, or Supply Chain) and describe a concise end-to-end use case demonstrating its value.

---

### **Q2 - (open_ended_theory_question)**

What is the measurable benefit delivered to the end user or system? Identify at least 3 KPIs this system could improve.

---

### **Q3 - (coding_question)**

Trace the complete data flow from document upload to query response. Identify each component, its responsibility, and the data transformations that occur.
Additionally, run this code in your local environment and identify bugs if any.

---

### **Q4 - (coding_question)**

Analyze the design decision to use an **in-memory ChromaDB** instance (no `persist_directory`). What are the implications, and how would you redesign for production?

---

### **Q5 - (open_ended_theory_question)**

Identify 3 scalability bottlenecks in this architecture. For each, propose a mitigation strategy suitable for handling 10,000+ documents.

---

### **Q6 - (coding_question)**

The chat history passed to the LLM has a format mismatch. Identify the bug in `app.py` and `RAG.py`, explain the issue, and provide the corrected code.

---

### **Q7 - (coding_question)**

The codebase lacks error handling. Write a robust `process_documents()` function that handles:
(a) empty file uploads, (b) API key validation, ( c) unsupported file types, and (d) ChromaDB connection failures.

---

### **Q8 - (coding_question)**

The application claims to support DOCX files, but the `requirements.txt` is missing critical dependencies. Identify the missing packages and explain why the current code would fail for DOCX files.

---

### **Q9 - (coding_question)**

Identify the typos and improvements needed in the system prompts in `RAG.py`. Rewrite the `system_prompt` with better structure and guardrails.

---

### **Q10 - (coding_question)**

Write pytest unit tests for the `DocumentProcessor` class covering:
(a) document loading, (b) text splitting with edge cases, and
(c) retriever creation with mocked embeddings.

---

### **Q11 - (coding_question)**

The current chunking strategy uses `CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)`. Explain why this is suboptimal and implement an improved strategy using at least 2 alternative techniques.

---

### **Q12 - (open_ended_theory_question)**

The current retriever uses basic similarity search with `k=5`. Propose 3 advanced retrieval techniques to improve answer quality, and explain the trade-offs of each.

---

### **Q13 - (coding_question)**

Replace the OpenAI dependency with a fully local LLM setup using Ollama. Provide the code changes needed in `RAG.py` and explain the architecture implications.

---

### **Q14 - (coding_question)**

List all the steps required to bring this project into a fully working state, including dependency fixes, configuration, and validation.

---

### **Q15 - (open_ended_theory_question)**

Create a PR request 

---
`GitHub Repository`: https://github.com/aays-tech-round/assignment-data-science-principal-ai-engineer

---

Note:
You can obtain an OpenAI trial API key for approximately $5 USD, which is sufficient to run and test the project end-to-end.

---


