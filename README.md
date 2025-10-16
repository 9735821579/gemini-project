# Automated LLM Code Deployment Agent (FastAPI/OpenAI)

This project implements a non-blocking API endpoint designed to receive a natural language coding task (a "brief"), utilize a large language model (LLM) to generate a web application, and automatically deploy that application to a GitHub Pages repository. The agent handles both the initial creation (Round 1) and subsequent revisions (Round 2) of the code.

The core functionality uses FastAPI for the API server, OpenAI (or a compatible LLM via the `openai` library) for code generation, and PyGithub for repository management.

## 🚀 Getting Started

### Prerequisites

1.  **Python 3.10+**
2.  **GitHub Personal Access Token (PAT):** Must have the `repo` and `workflow` scopes.
3.  **OpenAI API Key.**
4.  **Docker** (Recommended for deployment).

### 1. Project Setup

Clone the repository and install the dependencies:

```bash
# Clone your repository
git clone [https://github.com/YourUsername/gemini-project.git](https://github.com/YourUsername/gemini-project.git)
cd gemini-project

# Create a virtual environment and install dependencies
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt 
# Note: requirements.txt is a file you must create based on your imports.
