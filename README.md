# 🤖 Agentic AI Content Generation System

A multi-agent Agentic AI system built using **CrewAI and Python**, featuring specialized Planner, Writer, and Editor agents to generate structured, informative, and student-friendly educational blog articles for our clients Ramanujan Classes which operates for Classes 6–10.

## 📌 Project Overview

The Agentic AI Content Generation System automates the process of creating educational blog articles through collaboration between multiple AI agents.

Instead of relying on a single AI prompt, this project uses three specialized agents. Each agent has a specific responsibility and contributes to the overall content generation workflow.

The system is designed for **Ramanujan Classes**, an educational institute serving students from Classes 6 to 10.

## 🎯 Project Objectives

- Automate educational blog article generation.
- Implement a multi-agent architecture using CrewAI.
- Divide content creation into planning, writing, and editing tasks.
- Generate structured and easy-to-understand educational content.
- Reduce the manual effort involved in preparing educational articles.

## 🏗️ Multi-Agent Architecture

The project consists of three specialized AI agents working together in a sequential workflow.

### 1. Educational Content Planner

**Responsibility:** Article planning and structuring.

- Understands the given topic.
- Identifies important concepts and key points.
- Creates an organized article outline.
- Defines the structure and flow of the article.

### 2. Educational Content Writer

**Responsibility:** Article generation.

- Uses the planner's output.
- Develops the complete educational article.
- Explains concepts in simple English.
- Includes practical examples and learning tips.
- Organizes content using headings and subheadings.

### 3. Educational Content Editor

**Responsibility:** Article reviewing and refinement.

- Reviews the generated article.
- Improves grammar, spelling, and readability.
- Checks structure and clarity.
- Removes unnecessary repetition.
- Refines the final article for students in Classes 6–10.

## 🔄 Workflow

The system follows CrewAI's sequential execution process.

```text
       User Provides Topic
               |
               v
      Educational Planner
               |
               v
       Educational Writer
               |
               v
        Educational Editor
               |
               v
       Final Blog Article
               |
               v
       Manual Review
               |
               v
      Publish on Website
```

Each agent receives the output of the previous task, allowing the system to complete the article generation process in an organized manner.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| CrewAI | Multi-agent orchestration framework |
| OpenAI API | Large Language Model integration |
| Google Colab | Development and execution environment |
| Markdown | Generated article formatting |

## 📂 Project Structure

```text
crewai-agentic-content-generator/
│
├── Untitled4.ipynb
│
├── utils.py
│
├── README.md
│
├── requirements.txt
│
├── .gitignore
│
└── LICENSE
```

## ⚙️ Installation and Setup

### Prerequisites

- Python 3.10 or later
- OpenAI API key
- Google Colab or a local Python environment

### 1. Clone the Repository

```bash
git clone https://github.com/kishangithubkumar/crewai-agentic-content-generator.git
```

### 2. Navigate to the Project Directory

```bash
cd crewai-agentic-content-generator
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure the OpenAI API Key

The project uses a utility function to securely collect the API key at runtime.

```python
import os
from utils import get_openai_api_key

openai_api_key = get_openai_api_key()

os.environ["OPENAI_API_KEY"] = openai_api_key
```

Never hardcode or upload your actual API key to GitHub.

### 5. Run the Project

Open the Jupyter notebook:

```text
Untitled4.ipynb
```

Execute the notebook cells in sequence, configure your API key when prompted, and provide an educational topic to start the workflow.

## 📝 Sample Input

```python
inputs = {
    "topic": "Importance of Mathematics in Everyday Life"
}
```

## 📄 Sample Output

The system generates a complete educational blog article.

**Example:**

*Importance of Mathematics in Everyday Life: A Guide for Classes 6–10*

The generated article includes:

- Introduction
- Organized educational sections
- Practical mathematical examples
- Explanations of important concepts
- Student practice questions
- Answers and learning tips
- Conclusion

The generated article is reviewed manually before publication.

## 🔐 Security

- API keys are collected at runtime using `getpass()`.
- Actual API keys should never be committed to GitHub.
- Notebook outputs should be checked before uploading.
- Environment variables are used to configure API credentials.

## 🚀 Future Enhancements

Potential improvements for future versions include:

- Integration of live web-search tools for automated research.
- Source references and citations in generated articles.
- Improved factual verification.
- Automatic publishing to the institute's website.
- Article generation in multiple languages.

## 🎓 Learning Outcomes

Through this project, I explored:

- Agentic AI fundamentals.
- Multi-agent systems.
- CrewAI framework.
- AI agent roles, goals, and backstories.
- Task creation and task dependencies.
- Sequential agent execution.
- LLM integration using OpenAI.
- API key management and environment variables.

## 👨‍💻 Author

**Kishan Kumar**

- GitHub: [kishangithubkumar](https://github.com/kishangithubkumar)
- LinkedIn: [Kishan Kumar](https://www.linkedin.com/in/kishan-kumar-20228b261)

---

⭐ If you find this project interesting, consider giving the repository a star!

**Built with Python, CrewAI, and Agentic AI.**
