# Stock Market Analyst Agent (n8n workflow)

## Overview

This project implements an automated **Stock Market Analyst Agent** using n8n, Telegram, and AI-powered chart/image analysis. It allows users to:
- Request and receive stock market analysis via Telegram.
- Generate charts/images using HTTP APIs.
- Analyze images and interpret results using AI.
- Communicate interactively with the agent.

Two workflow models are included:
- **AA-1.1:** Event-based workflow, focuses on chart/image generation and Telegram notifications.

<img width="991" height="605" alt="Screenshot 2025-11-21 162817" src="https://github.com/user-attachments/assets/de8148a0-86da-4b21-b80b-a7ea6af4d567" />

- 
- **AA-1.2:** Conversation-based workflow, drives interaction using an integrated AI agent.

<img width="914" height="523" alt="Screenshot 2025-11-21 163252" src="https://github.com/user-attachments/assets/12d2bc9c-e97c-47ed-9679-fa547795a90b" />

## Features

- **Stock Data Analysis**: Automate chart/image generation with HTTP APIs.
- **Image Analysis**: AI interprets/describes generated chart images.
- **Telegram Integration**: Trigger, communicate, and receive data directly via Telegram bots.
- **AI Agent Model**: Utilizes Google Gemini for advanced market insights.
- **Extensible Workflows**: Easily add more endpoints, signals, or messaging platforms.

## Installation

### Requirements

- **n8n** (Self-hosted or Cloud)
- **Telegram Bot** (API Token + Username)
- **Node.js** (>=16.x recommended)
- Internet access for API requests

### Setup Steps

1. **Fork/Clone this repo**  
https://github.com/jeyaram1023/stock-market-analyst-n8n.git


2. **Install n8n**  
- Via npm:  
  ```
  npm install n8n -g
  ```
- Or use [Docker](https://hub.docker.com/r/n8nio/n8n).

3. **Start n8n**  
- Visit `http://localhost:5678` (default) in your browser.

4. **Import Workflows**
- Download the `.json` workflow files from this repo.
- In n8n UI, go to **Workflows > Import from File**, select the relevant file.

5. **Telegram Bot Setup**
- Create a bot via [@BotFather](https://core.telegram.org/bots#botfather).
- Copy your API token and set it in your n8n Telegram nodes.

6. **API Keys/Endpoints**
- Set your API endpoints (e.g., for chart generation) within the `HTTP Request` nodes.

## How to Run

1. **Trigger Event**  
- Use Telegram to send a message to your bot or execute workflow from another n8n workflow.

2. **Process Workflow**
- Workflow generates chart/image via external API.
- AI model analyzes chart/image.
- Bot sends result/analysis back to Telegram.

3. **Interact & Automate**
- Ask questions or request charts via Telegram.
- Get immediate market insights or chart breakdowns.

## Communication

- **Telegram Bot:** All analysis and communication is performed in Telegram.  
- For event-based actions (AA-1.1), send a signal from n8n or another workflow.
- For conversation (AA-1.2), type messages to your bot and receive automated replies.

- **Custom Endpoints:**  
- Extend workflows with new HTTP API endpoints for other financial data/chart services.

## Workflow Explanation

### AA-1.1: Event-Based Model
- Trigger: Executed by another workflow.
- Edit Fields: Prepares request data.
- HTTP Request: Sends data to chart/image API.
- Analyze Image: AI interprets the generated image.
- Telegram: Sends analysis to your chat.
- Edit Fields1: Further manual edits as required.

### AA-1.2: Chat-Based Model
- Telegram Trigger: Listens for incoming messages.
- AI Agent: Handles chat communication using Google Gemini, window buffer memory, and chart tools.
- Telegram: Responds with message/analysis.

## Customization

- Replace `HTTP Request` endpoints with your preferred chart or data APIs.
- Customize AI agent with any LLM or plugin supported by n8n.
- Add more platforms or integrations (Discord, WhatsApp, etc.).

## Contact

For questions, requests, collaboration, or support, contact **Jeyaram Reddy**:

- **Email:** jeyaram.reddy.ece@gmail.com
- **Telegram:** [@JeyaramReddy1023](https://t.me/JeyaramReddy1023)
- **GitHub Profile:** [jeyaram1023](https://github.com/jeyaram1023)
- **Location:** Kavali, Andhra Pradesh, India

## License

This repository is open source and freely available for use, modification, and distribution.  
_Consider giving credit if you use or modify the workflows._

## Screenshots

Include the provided screenshots in your repo as reference for workflow design:

<img width="914" height="523" alt="Screenshot 2025-11-21 163252" src="https://github.com/user-attachments/assets/c02d99ce-8845-4def-802e-4a1711ddaf28" />
<img width="966" height="589" alt="Screenshot 2025-11-21 162900" src="https://github.com/user-attachments/assets/55bb6beb-bb80-4469-be0a-bde8f5db7685" />

![Screenshot_20251121_161351](https://github.com/user-attachments/assets/d2ae141d-b0e8-4e05-82cb-b7de2aca765f)


## Contribution

Pull requests are welcome! If you'd like to extend functionality, improve documentation, or fix bugs, please submit a PR or email.

**Happy Automating!**
