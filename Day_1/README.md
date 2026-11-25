----This is the task of day_1----

# Task Description
This task focuses on setting up and connecting a Large Language Model (LLM) using **Groq and LangChain** in Google Colab.It demonstrates how to install the required library, securely access the Groq API key, and initialize an AI language model.

# Objectives
- Install and configure the `langchain_groq` package.
- Import the `ChatGroq` class for LLM integration.
- Securely retrieve the Groq API key using Google Colab Secrets.
- Configure the language model with appropriate parameters.
- Initialize the LLM for AI-based applications.

# Technologies Used
- Python
- Google Colab
- LangChain
- Groq API
- Groq LLM (`openai/gpt-oss-120b`)

# Implementation
1. Install Required Library
Install the LangChain Groq integration package.

 2. Import Required Libraries
Import `ChatGroq`, Python's `os` module, and Google Colab's `userdata`.

 3. Configure API Key
Retrieve the Groq API key securely from Google Colab Secrets and store it as an environment variable.

 4. Initialize the Language Model
Create a ChatGroq instance using the selected model and configure its temperature.

# Expected Outcome
Successfully installs the LangChain Groq integration, retrieves the API key securely, and initializes the Groq language model for further AI application development.

#Conclusion
This task demonstrates the basic setup required to integrate a Groq-hosted language model with LangChain using Python. It establishes the foundation for building AI-powered applications and interacting with LLMs.
