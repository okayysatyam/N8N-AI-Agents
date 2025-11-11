#  N8N AI Agents



![N8N Logo](https://raw.githubusercontent.com/n8n-io/n8n/master/assets/n8n-logo.png) <!-- TODO: Add a more specific project logo if available -->
<div>

## Overview

As a freelancer, I have made various Automations & Workflows for different clients. These are some of the most loved workflows. This repository provides a curated collection of n8n workflows designed to harness the power of Artificial Intelligence for various automation tasks. 
Built with [n8n](https://n8n.io/), a powerful workflow automation tool, these "AI Agents" enable users to integrate advanced AI capabilities easily 
into their business processes, personal projects, and operational workflows without writing extensive code.

## Table of Contents

- [Key Capabilities](#key-capabilities)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Workflows](#workflows)
- [Quick Start](#quick-start)
- [Use Cases by Industry](#use-cases-by-industry)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Key Capabilities

- **Code When You Need It:** Write JavaScript/Python, add npm packages, or use the visual interface.
- **AI-Native Platform:** Build AI agent workflows based on LangChain with your own data and models.
- **Modular Automations:** Combine AI, APIs, and logic nodes into reusable workflow components.
- **Seamless Integrations:** Connect with 400+ apps including Gmail, Slack, OpenAI, Google Calendar, Twilio, and more.
- **Deploy Anywhere:** Run locally, in Docker, or on n8n Cloud with full data ownership.

## Tech Stack

- **Workflow Automation:** n8n ![n8n](https://img.shields.io/badge/n8n-FF5722?style=for-the-badge&logo=n8n&logoColor=white)
- **AI Models:** OpenAI (GPT-4, GPT-4o), Google Gemini, Ollama (local LLMs)
- **Voice & Audio:** ElevenLabs, OpenAI Whisper, Twilio
- **Integrations:** Gmail, Google Calendar, Google Sheets, Slack, Strava, Supabase, PostgreSQL
- **Frameworks:** LangChain for AI agent orchestration

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

## Workflows

### Chatbots & Conversational AI

#### 1. AI Voice Agent
**Use Case:** Intelligent voice-based appointment booking and customer interaction  
**Integrations:** Twilio + OpenAI GPT-4 + Google Sheets  
**Features:**
- Receive voice calls via Twilio webhook
- Extract phone information and voice message content
- Process natural language with OpenAI to understand intent
- Detect appointment-related keywords automatically
- Send intelligent SMS responses via Twilio
- Log conversations and interactions to Google Sheets
- Support for appointment booking flow triggers

#### 2. Chat with Local LLMs using n8n and Ollama
**Use Case:** Private, self-hosted conversational AI without external API dependencies  
**Integrations:** Ollama + Local LLM Models  
**Features:**
- Connect to locally hosted Ollama server
- Chat interface with self-hosted language models
- Complete data privacy—no external API calls
- Support for multiple open-source LLM models
- Docker-compatible deployment
- Zero latency concerns with local processing

#### 3. InstaTest Chatbot
**Use Case:** Interactive chatbot for automated testing and customer engagement  
**Integrations:** n8n Chat Interface + AI Models  
**Features:**
- Instant response generation
- Context-aware conversations
- Multi-turn dialogue support
- Customizable persona and tone


### Data & Business Intelligence

#### 4. Automation for Realtime Insights on Meetings
**Use Case:** AI-powered meeting transcription and real-time insights generation  
**Integrations:** Recall.ai + OpenAI Assistants + Supabase/PostgreSQL + AssemblyAI  
**Features:**
- Automatically join meetings (Zoom, Google Meet, Teams)
- Real-time transcription with speaker identification
- Keyword detection triggers ("Jimmy" activates AI assistant)
- Structured dialogue storage in database
- AI note-taking on command
- Meeting summary generation
- Persistent thread management with OpenAI Assistants
- Automatic silence and bot detection for smart leaving

#### 5. Automation to Find YouTube Trends on Niche
**Use Case:** Market research and content strategy through YouTube trend analysis  
**Integrations:** YouTube Data API + AI Analysis  
**Features:**
- Search trending videos in specific niches
- Extract video metadata and engagement metrics
- AI-powered trend analysis and insights
- Identify content opportunities
- Track competitor performance

#### 6. Daily Meetings Summarization with Gemini AI
**Use Case:** Automated daily meeting summary sent to team channels  
**Integrations:** Google Calendar + Google Gemini Flash + Slack  
**Features:**
- Schedule trigger (runs daily at 9 AM)
- Retrieve today's calendar events automatically
- AI agent with calendar retrieval tool
- Generate concise meeting summaries
- List all attendees for each meeting
- Send formatted summary to Slack channel
- Custom date range queries supported

#### 7. Vector Database as Big Data Analysis Tool for AI Agents
**Use Case:** Semantic search and AI-powered data analysis on large datasets  
**Integrations:** Vector Database + LangChain + OpenAI Embeddings  
**Features:**
- Store and index large volumes of text data
- Semantic similarity search
- Context-aware AI responses
- RAG (Retrieval Augmented Generation) implementation
- Efficient large-scale data querying


### Operations & HR

#### 8. Gmail AI Autoresponder: Draft Replies
**Use Case:** Intelligent email management with AI-generated draft responses  
**Integrations:** Gmail + OpenAI GPT-4 + OpenAI GPT-4 Turbo  
**Features:**
- Trigger on new incoming emails (excludes own emails)
- AI assessment to determine if reply is needed
- Filter out marketing emails automatically
- Generate contextual, professional draft replies
- Support for yes/no questions (provides both options)
- Business casual tone with proper email structure
- Saves drafts in Gmail thread (doesn't auto-send)
- Multi-language response support
- Placeholder generation for unknown information

#### 9. HR-Focused Automation Pipeline with AI
**Use Case:** Automated CV screening and candidate evaluation  
**Integrations:** n8n Form + OpenAI GPT-4o-mini + Google Drive + Google Sheets  
**Features:**
- Form submission for CV upload (PDF only)
- Automatic CV upload to Google Drive
- Extract text from PDF resumes
- AI-powered information extraction (education, job history, skills, contact info)
- Candidate profile summarization
- Match candidate against job requirements
- Automated scoring (1-10 scale) with reasoning
- Store complete evaluation in Google Sheets
- Structured data output for HR review

#### 10. Human in the Loop System: Email Response with AI
**Use Case:** AI-assisted email responses with human approval before sending  
**Integrations:** Gmail + OpenAI + Approval Workflow  
**Features:**
- AI generates initial email drafts
- Human review and edit capability
- Approval gate before sending
- Context preservation across conversation threads
- Quality control for customer-facing communications


### Sales & CRM Automation

#### 11. Appointment Scheduling AI
**Use Case:** Intelligent multi-step appointment booking with AI qualification  
**Integrations:** n8n Multi-page Forms + OpenAI + Gmail + Google Calendar  
**Features:**
- Multi-page form experience for better UX
- AI-powered enquiry classification (relevant vs. irrelevant)
- Decline non-qualifying requests with alternative options
- Terms and conditions acceptance step
- Dynamic date selection (next 5 weekdays)
- Time slot selection (9 AM - 6 PM)
- Email acknowledgement to requester
- AI summarisation of enquiry for admin
- Gmail wait-for-approval workflow (confirm/decline buttons)
- Automatic Google Calendar event creation on approval
- Rejection notification email
- Sub-workflow pattern for approval process

#### 12. Sales Agent Automation
**Use Case:** Automated lead qualification and follow-up sequences  
**Integrations:** CRM + Email + AI Analysis  
**Features:**
- Lead scoring and prioritization
- Personalized outreach generation
- Follow-up sequence automation
- Pipeline stage management

#### 13. Social Media Analysis and Automated Email Generation
**Use Case:** Monitor social media activity and generate personalized outreach  
**Integrations:** Social Media APIs + OpenAI + Email Service  
**Features:**
- Track prospect social media activity
- Analyze engagement patterns
- Generate contextual outreach emails
- Timing optimization for sending
- Multi-platform monitoring



#### 14. Fitness Coach Automation
**Use Case:** AI-powered triathlon coaching with personalized workout analysis  
**Integrations:** Strava + Google Gemini 2.0 Flash + Google Sheets + Email/WhatsApp  
**Features:**
- Strava activity trigger (runs, swims, bikes)
- Comprehensive activity data extraction
- AI triathlon coach with specialized knowledge
- Multi-sport analysis (swimming, cycling, running)
- Activity-specific metrics evaluation (pace, heart rate, cadence, power, SWOLF)
- Personalized coaching feedback and recommendations
- Workout improvement suggestions
- Training load balancing across disciplines
- Brick workout recommendations
- HTML-formatted coaching reports
- Multi-channel delivery (Email, WhatsApp, Google Sheets)
- Activity logging with AI feedback in spreadsheet


#### 15. Automation to Translate Audio from AI
**Use Case:** Multi-language audio translation pipeline  
**Integrations:** ElevenLabs + OpenAI Whisper + OpenAI Chat + LangChain  
**Features:**
- Text-to-speech generation in source language (French)
- Audio transcription with Whisper
- AI-powered text translation (French to English)
- Translated text-to-speech generation
- Multi-voice support via ElevenLabs
- Complete audio translation workflow
- High-quality voice synthesis

---

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
  

## Use Cases by Industry

- **Customer Service:** AI chatbots, email autoresponders, voice agents
- **HR & Recruitment:** CV screening, candidate evaluation, interview scheduling
- **Sales & Marketing:** Lead qualification, social media analysis, appointment booking
- **Operations:** Meeting transcription, daily summaries, document processing
- **Health & Fitness:** Personalized coaching, activity analysis, progress tracking
- **Content Creation:** Translation services, voice synthesis, trend analysis
  
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

- [n8n.io](https://n8n.io) for creating a versatile workflow automation platform
- The n8n community for continuous inspiration and best practices
- All contributors who helped build and refine these workflows

