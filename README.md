# 🚀 Autonomous AI Coding Agent

An autonomous multi-agent AI system that generates full-stack applications from a single user prompt, automatically executes the generated project, tests backend APIs, identifies failures, analyzes root causes, plans repairs, debugs the code, and retries until the application works or the retry limit is reached.

Developed by **Ankit Kumar Gupta**.

---

# 🌟 Features

* 🏗️ Automatic project architecture generation
* 📋 Project specification generation
* 📂 File responsibility (contract) generation
* 🔄 Dependency-aware code generation
* ⚡ Backend generation in iterative order
* 🎨 Frontend generation using extracted API contracts
* 📄 Automatic file creation
* 📦 Dependency validation
* ▶️ Automatic project execution
* 🧪 Automatic backend API testing
* 🔍 Rule-based error analysis
* 📑 Debug planning
* 🧠 Context-aware debugging
* 🔁 Self-healing retry loop
* 🛑 Automatic termination after successful execution or maximum retries

---

# 🏛️ Multi-Agent Architecture

| Agent                     | Responsibility                                   |
| ------------------------- | ------------------------------------------------ |
| Architecture Agent        | Creates project structure                        |
| Project Spec Agent        | Generates complete project specification         |
| File Contract Agent       | Defines responsibility and exports of every file |
| Generation Order Agent    | Creates dependency-aware generation order        |
| Create Files Agent        | Creates project folders and empty files          |
| Backend Generation Agent  | Generates backend files iteratively              |
| API Contract Agent        | Extracts API schema from generated backend       |
| Frontend Generation Agent | Generates frontend using API contract            |
| Validation Agent          | Validates generated code                         |
| Dependency Agent          | Installs required dependencies                   |
| Run Agent                 | Executes backend and frontend                    |
| API Test Agent            | Tests every backend API automatically            |
| Error Analysis Agent      | Detects structured errors and root causes        |
| Debug Planning Agent      | Groups failures and prepares repair plan         |
| Context Builder Agent     | Builds debugging context for LLM                 |
| Debug Agent               | Repairs faulty code using contextual reasoning   |

---

# 🔄 Workflow

```text
                    START
                       │
                       ▼
            Architecture Agent
                       │
                       ▼
           Project Specification Agent
                       │
                       ▼
             File Contract Agent
                       │
                       ▼
           Generation Order Agent
                       │
                       ▼
              Create Files Agent
                       │
                       ▼
        Backend Generation Agent
                       ▲
                       │
        (loops until backend complete)
                       │
                       ▼
             API Contract Agent
                       │
                       ▼
       Frontend Generation Agent
                       ▲
                       │
      (loops until frontend complete)
                       │
                       ▼
              Validation Agent
                       │
                       ▼
              Dependency Agent
                       │
                       ▼
                  Run Agent
                       │
                       ▼
               API Test Agent
                       │
        ┌──────────────┴──────────────┐
        │                             │
        │ APIs Pass                   │ APIs Fail
        │                             │
        ▼                             ▼
       END                 Error Analysis Agent
                                      │
                                      ▼
                             Debug Planning Agent
                                      │
                                      ▼
                            Context Builder Agent
                                      │
                                      ▼
                                Debug Agent
                                      │
                                      ▼
                                 Run Agent
                                      │
                               (Retry Loop)
```

---

# 🧠 Debugging Pipeline

```
API Test Agent
        │
        ▼
Error Analysis Agent
        │
        ▼
Debug Planning Agent
        │
        ▼
Context Builder Agent
        │
        ▼
Debug Agent
        │
        ▼
Run Agent
        │
        ▼
API Test Agent
```

The debugging loop continues until:

* All API tests pass
*  Maximum retry count is reached

---

# ⚙️ Tech Stack

* Python
* LangGraph
* LangChain
* Groq LLM (Llama 3.3 70B Versatile)
* Flask
* MongoDB


---

# Installation

```bash
git clone https://github.com/yourusername/Autonomous-Coding-Agent.git

cd Autonomous-Coding-Agent

pip install -r requirements.txt
```

---


---

# Example Prompt

```
Create a Todo application using Flask, MongoDB, HTML, CSS and JavaScript.
```

The agent will automatically:

* Design the architecture
* Generate all files
* Generate backend
* Extract API contract
* Generate frontend
* Execute the project
* Test APIs
* Detect failures
* Debug automatically
* Retry execution

without human intervention.

---

# Future Improvements

* Browser automation testing
* Screenshot-based UI debugging
* Docker support
* Kubernetes deployment
* Vector memory for debugging history
* Multi-file repair planning
* Human approval mode
* CI/CD integration

---

# Author

## **Ankit Kumar Gupta**

AI/ML Engineer | Generative AI Developer | Multi-Agent Systems | LangGraph | RAG | Backend Development




