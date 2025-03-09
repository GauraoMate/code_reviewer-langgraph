# Code Reviewer API

This project implements a **Code Reviewer API** using **LangChain**, **LangGraph**, and **Groq's LLM**. It leverages a graph-based state management system to generate Python code for a given task, conduct peer reviews, and evaluate the code quality.

## Features

- **Code Generation**: Automatically generate Python code based on a given task description.
- **Peer Review**: Perform peer review on the generated code using LLM.
- **Code Rewriting**: Rewrite the code based on peer review feedback.
- **Evaluation**: Score and summarize the code quality.
- **Graph-Based Workflow**: Uses LangGraph to manage multi-step processes.

## Tech Stack
- **Python**
- **LangChain**
- **LangGraph**
- **Groq LLM**
- **Dotenv** for managing environment variables

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up your environment variables by creating a `.env` file in the root directory:
   ```plaintext
   GROQ_API_KEY=<your-groq-api-key>
   ```

## Usage

1. Run the Jupyter Notebook to initiate the code review process.
2. The notebook follows a multi-step process:
   - **Code Generation**: Generates Python code based on a task description.
   - **Peer Review**: Reviews the code and provides feedback.
   - **Code Rewriting**: Refines the code based on feedback.
   - **Evaluation**: Scores and summarizes the code quality.

3. The output will include:
   - **Generated Code**
   - **Peer Review Feedback**
   - **Rewritten Code**
   - **Code Quality Score and Summary**

## Example Workflow

1. **Input Task Description**: Provide a task description.
2. **Generate Code**: The LLM generates code.
3. **Peer Review**: The LLM provides feedback on the code.
4. **Rewrite Code**: The LLM rewrites the code based on feedback.
5. **Evaluate Code**: The LLM provides a score and summary.

## Environment Variables

Ensure you set the following environment variable in your `.env` file:

```plaintext
GROQ_API_KEY=<your-groq-api-key>
```

