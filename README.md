# PromptEngAssignment

Running LLMs Locally: Llama3 and Gemma7B
This repository contains instructions and scripts to set up and run two language models (LLMs), Llama3 and Gemma7B, locally on your machine. By following this guide, you'll be able to interact with both models using the curl command.

Table of Contents
Introduction
Prerequisites
Setup Instructions
Llama3
Gemma7B
Usage
Comparison
Repository Structure
Video Demonstration
Conclusion
References
Introduction
This project demonstrates how to download, install, and run two large language models, Llama3 and Gemma7B, on a local machine. The goal is to interact with these models using the curl command and compare their performance on identical prompts.

Prerequisites
Before you begin, ensure you have the following installed on your system:

Python 3.7 or higher
Git
Docker (recommended for easier setup)
curl
A suitable text editor or IDE (e.g., VSCode)
Setup Instructions
Llama3
Download Llama3: Follow the instructions on the official Llama3 to download and set up the model.

Install Dependencies:

pip install -r requirements.txt

Run Llama3 Model:
python run_llama3.py

Verify Setup: You can verify if Llama3 is running correctly by using the curl command:
curl -X POST http://localhost:5000/predict -d '{"prompt": "Hello, Llama3!"}'

Gemma7B
Download Gemma7B: Follow the instructions on the official Gemma7B to download and set up the model.
Install Dependencies:
pip install -r requirements.txt

Run Gemma7B Model:
python run_gemma7b.py

Verify Setup: Similar to Llama3, verify the setup using curl:
curl -X POST http://localhost:6000/predict -d '{"prompt": "Hello, Gemma7B!"}'

Usage
After setting up both models, you can interact with them via the curl command.

Llama3 Interaction
curl -X POST http://localhost:5000/predict -d '{"prompt": "Tell me a joke."}'

Gemma7B Interaction
curl -X POST http://localhost:6000/predict -d '{"prompt": "Tell me a joke."}'

Comparison
To compare the performance of both models, you can pass the same prompt to each model and observe their responses. This helps in understanding the strengths and weaknesses of each model.

Repository Structure
. ├── llama3/ │ ├── run_llama3.py │ ├── requirements.txt │ └── ... ├── gemma7b/ │ ├── run_gemma7b.py │ ├── requirements.txt │ └── ... ├── README.md └── setup_instructions.md

Video Demonstration
A video demonstration of setting up and interacting with both models is available at: YouTube Link

Conclusion
This project provided hands-on experience in setting up and running LLMs locally. By comparing the responses from Llama3 and Gemma7B, we gained insights into their capabilities and performance.

References
Llama3
Gemma7B
Medium Article: 50 Open Source Options for Running LLMs Locally
