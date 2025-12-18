## **A. Architecture Question **

**Architecture & Scalability Assessment**

Define the business problem this codebase solves in a domain of your choice (e.g., CPG, Manufacturing, Retail, Pharma, or Supply Chain) and describe a concise end-to-end use case.
Evaluate the current architecture’s ability to handle **10,000+ documents**, identify measurable benefits (at least **3 KPIs**), and propose a **scalable redesign** highlighting key architectural changes, trade-offs, and system components.

---

## **B. Coding Question **

**End-to-End System Execution, Debugging, and Enhancement**

Run the project locally and perform the following **coding tasks** without changing the functional intent of the system:

1. Trace and document the **complete data flow** from document upload to query response, identifying each component, responsibility, and data transformation.
2. Identify and fix **runtime bugs and missing dependencies** (including DOCX support failures).
3. Implement a robust `process_documents()` function with handling for:

   * empty file uploads
   * API key validation
   * unsupported file types
   * ChromaDB connection failures
4. Replace the existing chunking logic (`CharacterTextSplitter`) with an **improved chunking strategy** using at least **two alternative techniques**, implemented in code.
5. Replace the OpenAI dependency with a **fully local LLM setup using Ollama**, modifying `RAG.py` accordingly and ensuring the system runs end-to-end.
6. Provide the **exact steps and code changes** required to bring the project into a fully working, production-ready state (dependencies, configuration, validation).

> **Note:** This is a coding exercise - focus on implementation, not theory.

---


## **C. GitHub PR & Submission Instructions**

1. Fork the repository:
   **GitHub Repository:** [https://github.com/aays-tech-round/assignment-data-science-principal-ai-engineer](https://github.com/aays-tech-round/assignment-data-science-principal-ai-engineer)

2. Create a feature branch with a clear and descriptive name.

3. Implement all required **architecture and coding changes**.

4. Add an `answers.md` file at the root of the repository containing:

   * **Architecture question answers**
   * Architecture rationale, scalability discussion, KPIs, and redesign proposal

5. Add **coding question explanations** to the **same `answers.md` file**, including:

   * A brief description of each fix or enhancement
   * **Exact file names** where changes were made
   * Any assumptions or limitations

6. Ensure all **code changes are fully implemented in the repository**, not just described.

7. Commit changes with meaningful, atomic commit messages.

8. Raise a **single Pull Request** that includes:

   * All code changes
   * `answers.md`
   * Clear PR description summarizing:

     * What was fixed
     * What was improved
     * How to run and validate the project end-to-end

9. The project must run successfully end-to-end in a local environment.


---

### **Note**

You may use an **OpenAI trial API key (~$5 USD)** if needed to validate the original flow before replacing it with a local LLM.

---



