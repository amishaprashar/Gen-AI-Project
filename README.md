# Gen-AI-Project
 
---
# GenAI Dockerfile Generator

This project uses **Large Language Models (LLMs)** to automatically generate **Dockerfiles for different programming languages** based on user prompts.
Users can modify the prompt to customize the Dockerfile according to their application requirements.

The project supports two types of LLM integrations:

* **Hosted LLM (Google Gemini)**
* **Local LLM (Ollama)**

---

# Project Structure

```
genai-dockerfile-generator/
│
├── hosted-llm-gemini/
│   ├── generate_dockerfile.py
│   └── requirements.txt
│
├── local-llm-ollama/
│   ├── generate_dockerfile.py
│   └── requirements.txt
│
└── README.md
```

---

# Features

* Generate Dockerfiles for **multiple programming languages**
* Supports **hosted and local LLMs**
* **Customizable prompts** for flexible Dockerfile generation
* Simple **Python-based implementation**

---

# Setup Instructions

## 1️⃣ Clone the Repository

```bash
git clone <repository-url>
cd Gen-AI-Project
```

---

# Using Hosted LLM (Gemini)

### Step 1: Navigate to the folder

```bash
cd hosted-llm-gemini
```

### Step 2: Install dependencies

```bash
pip3 install -r requirements.txt
```

### Step 3: Configure API Key

Set your **Google Gemini API Key** as an environment variable.

```bash
export GEMINI_API_KEY=your_api_key
```

### Step 4: Run the script

```bash
python3 generate_dockerfile.py
```

---

# Using Local LLM (Ollama)

### Step 1: Install Ollama

Install Ollama from:

[https://ollama.com](https://ollama.com)

---

### Step 2: Pull a model

Example:

```bash
ollama pull llama3.2:1b
```

---

### Step 3: Navigate to the folder

```bash
cd local-llm-ollama
```

---

### Step 4: Install dependencies

```bash
pip3 install -r requirements.txt
```

---

### Step 5: Run the script

```bash
python3 generate_dockerfile.py
```

---

# Example Workflow

1. User selects a programming language (e.g., Python, Node.js).
2. The script sends a prompt to the LLM.
3. The LLM generates a **Dockerfile** based on the prompt.
4. The user can modify the prompt to customise the output.

---

# Example Prompt

```
Generate a production-ready Dockerfile for a Python Flask application.
```

---

# Tech Stack

* Python
* Large Language Models (LLMs)
* Google Gemini API
* Ollama (Local LLM)
* Docker

---

# Future Improvements

* Web UI for prompt input
* Support for more LLM providers
* Advanced Dockerfile optimisation
* Kubernetes deployment template generation

 
