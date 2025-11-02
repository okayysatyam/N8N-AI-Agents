#  N8N AI Agents



![N8N Logo](https://raw.githubusercontent.com/n8n-io/n8n/master/assets/n8n-logo.png) <!-- TODO: Add a more specific project logo if available -->
<div>

## Overview

As a freelancer, I have made various Automations & Workflows for different clients. These are some of the most loved workflows. This repository provides a curated collection of n8n workflows designed to harness the power of Artificial Intelligence for various automation tasks. 
Built with [n8n](https://n8n.io/), a powerful workflow automation tool, these "AI Agents" enable users to easily integrate advanced AI capabilities 
into their business processes, personal projects, and operational workflows without writing extensive code.

## Table of Contents

- [Key Capabilities](#key-capabilities)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Quick Start](#quick-start)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Key Capabilities

- **Code When You Need It:** Write JavaScript/Python, add npm packages, or use the visual interface.
- **AI-Native Platform:** Build AI agent workflows based on LangChain with your own data and models.
- **Modular Automations:** Combine AI, APIs, and logic nodes into reusable workflow components that scale from quick prototypes to production pipelines.
- **Seamless Integrations:** Connect instantly with 400+ apps and services — from Google Workspace and Slack to OpenAI and Whisper — without custom coding.
- **Deploy Anywhere:** Run locally, in Docker, or on n8n Cloud with full data ownership and version-controlled workflow exports.

## Tech Stack

-   **Workflow Automation:** n8n ![n8n](https://img.shields.io/badge/n8n-FF5722?style=for-the-badge&logo=n8n&logoColor=white)
-   **AI Integration:** Large Language Models (LLMs) & AI Services (e.g., OpenAI, Google AI, Ollmma etc.)

## Project Structure

```
├── Chatbots & Conversational AI/
│   ├── n8n chatbot
│   ├── Chat with local LLMs using n8n and Ollama
│   └── InstaTest
├── Data & Business Intelligence/
│   ├── Automation for realtime insights on meetings
│   ├── Automation to find youtube trend on niche
│   ├── Daily meetings summarization with Gemini AI
│   └── Vector Database as a Big Data Analysis Tool for AI Agents
├── Operations & HR/                          # Directory for operations and HR workflows
│   ├── Gmail AI autoresponder_ draft replies
│   ├── HR-focused automation pipeline with AI
│   └── Human in the loop system email response with AI
├── Sales & CRM Automation/                   # Directory for sales and CRM automation workfents/
│   ├── Sales Agent Automation
│   ├── Appointment Scheduling AI
│   └── Social Media Analysis and Automated Email Generation
├── .gitignore
├── AI Voice Agent.json                       # n8n workflow for AI Voice Agents
├── Automation to translate audio from AI.json # n8n workflow for AI-powered audio translation
├── Chatbots & Conversational AI/             # Dirlows
├── Fitness coach Automation.json             # n8n workflow for fitness coach automation
├── LICENSE
└── README.md
```

##  Quick Start

To use these workflows, you'll need an active n8n instance.

### Prerequisites

-   An active n8n instance (self-hosted or n8n Cloud).
    -   [Setup n8n Locally](https://docs.n8n.io/getting-started/installation/installation-methods/binary/)
    -   [Setup n8n with Docker](https://docs.n8n.io/getting-started/installation/installation-methods/docker/)
    -   [n8n Cloud](https://n8n.io/cloud/)

### Installation (Importing Workflows)
   **Deploy with Docker**
   ```bash
   docker volume create n8n_data
   docker run -it --rm --name n8n -p 5678:5678 -v n8n_data:/home/node/.n8n docker.n8n.io/n8nio/n8n
   ```
   OR
   
1.  **Clone the repository**
    ```bash
    git clone https://github.com/okayysatyam/N8N-AI-Agents.git
    cd N8N-AI-Agents
    ```

2.  **Open your n8n instance**
    Access your n8n UI (e.g., `http://localhost:5678`).

3.  **Import a Workflow**
    -   In the n8n UI, click on the **"Workflows"** tab.
    -   Click on **"New"** then **"Import from JSON"** or **"Import Workflow"**.
    -   Copy the content of any `.json` file from this repository (e.g., `AI Voice Agent.json`) and paste it into the import dialogue.
    -   Click **"Import"**.

4.  **Configure Credentials & Activate**
    -   Once imported, the workflow will appear in your list.
    -   Many AI-powered workflows require credentials for services like OpenAI or other LLM providers. Open the imported workflow, locate the nodes requiring credentials (e.g., "OpenAI" node), and set up your API keys.
    -   After configuring necessary credentials, **activate** the workflow using the toggle switch in the top right corner of the workflow editor.

5.  **Test the Workflow**
    -   You can manually test the workflow by clicking "Execute Workflow" or trigger it via its configured start node (e.g., a webhook, a schedule).
  
## Contributing

We welcome contributions to expand this collection! If you have an n8n AI Agent workflow you'd like to share, please consider:

1.  Forking the repository.
2.  Creating a new branch (`git checkout -b feature/your-workflow`).
3.  Adding your `.json` workflow file, preferably categorized into an existing or new directory.
4.  Adding a brief description of your workflow to the `Features` section of this README.
5.  Opening a Pull Request.

Please ensure your workflows are well-documented within n8n, and any required external credentials are clearly indicated.

## License

This project is licensed under the [MIT License](LICENSE) - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

-   [n8n.io](https://n8n.io/) for creating such a versatile workflow automation tool.

This repository is a testament to the power of the n8n community and the rapid evolution of practical AI. The patterns demonstrated here are
inspired by the real-world business challenges solved and shared by automation engineers and developers every day.
