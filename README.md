# 🟧 Stock Market Analyst Automation System


---

<p align="center">
  <img src="https://img.shields.io/badge/Project-Verified-blue.svg?style=for-the-badge" />
  <img src="https://img.shields.io/badge/n8n-Automation-success?style=for-the-badge&logo=data:image/svg+xml;base64," />
  <img src="https://img.shields.io/badge/Telegram-Active-blue?style=for-the-badge&logo=telegram" />
  <img src="https://img.shields.io/badge/Gemini-Integrated-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-orange?style=for-the-badge" />
</p>

---

## 🟧 1. Project Overview

Automated Stock Market Analyst built using **n8n workflow automation**, **Telegram Bot**, and **AI-powered chart/image analysis**.  
Generates stock charts, analyzes with Gemini, and interprets results—delivered right into Telegram.  
Supports both event-driven and chat-based market analysis using a user-friendly agent model.

---

## 🟧 2. System Architecture Diagram


<img width="914" height="523" alt="Screenshot 2025-11-21 163252" src="https://github.com/user-attachments/assets/c9e4d12e-135b-4708-aa8c-260b70c92b45" />
<img width="966" height="589" alt="Screenshot 2025-11-21 162900" src="https://github.com/user-attachments/assets/7bc232be-b878-40e0-817a-23899b9f5cff" />


---

## 🟧 3. Technology Stack

- **n8n**: Visual, code-free workflow automation
- **Telegram Bot**: User interaction & results delivery
- **Google Gemini AI**: Powerful chart/image interpretation
- **HTTP API chart services**: Data visualization
- **HTML / JS**: (Optional) Portal for advanced triggers

---

## 🟧 4. Features

- Generates market charts automatically via API
- AI analyzes and explains chart images
- Delivers instant insights and updates via Telegram
- Event-driven (AA-1.1) or chat-based (AA-1.2) analysis flows
- Easily customizable and extensible
- Quick integration with more APIs/data feeds

---

## 🟧 5. Sample Data and Workflow Files

- **Sample Workflow**: Provided as JSON export, ready to import into n8n
- **Images for Reference**:
- ![generated-image (1)](https://github.com/user-attachments/assets/f195f5f2-ff05-4ff4-b779-3a2a6df94679)

- **How to Import**:
  1. Open n8n dashboard
  2. Click "Import Workflow"
  3. Upload workflow JSON, review node config

---

## 🟧 6. Setup Guide

1. **Clone this repo**
git clone https://github.com/jeyaram1023/stock-market-analyst-n8n.git
cd stock-market-analyst-n8n
2. **Install n8n**
npm install n8n -g

n8n
- Open `http://localhost:5678` in browser

3. **Telegram Bot Setup**
- Create bot using [@BotFather](https://t.me/botfather)
- Set bot token in n8n Telegram node

4. **Import Workflow**
- Go to Workflows > Import from File
- Select provided JSON, connect nodes

5. **Configure HTTP API**
- Chart generation endpoints set in HTTP Request node
- Add API key if required

---

## 🟧 7. How It Works

- **AA-1.1 (Event Model):**  
1. Triggered by other workflow or manual execution
2. Generates and fetches chart image via HTTP API
3. AI analyzes image for insights
4. Telegram bot sends message with chart + analysis

- **AA-1.2 (Chat Model):**  
1. User sends query to Telegram bot
2. AI Agent (Gemini) interprets request
3. Workflow fetches/generates chart & analyzes
4. Result delivered in chat with context memory

---

## 🟧 8. Communication

- All user-facing messages via Telegram bot
- Fully interactive chat for stock queries, follow-ups
- Event signals trigger analysis workflows instantly

---

## 🟧 9. Customization

- Change chart API endpoints as needed
- Plug in any AI service supported by n8n (OpenAI, Gemini, etc.)
- Add more triggers: Discord, WhatsApp, Email alert, etc.

---

## 🟧 10. Example Telegram Output

> 📊 Stock Chart:
> ![stock_assignment_telegram](https://github.com/user-attachments/assets/74db4624-d709-40df-b7e2-0f5a77b2bd0d)

> <img width="800" height="600" alt="9e3752f2-bfb4-42b6-a8f7-af646dccf191" src="https://github.com/user-attachments/assets/c64aba83-1e33-4f1d-b295-1ed4460927ef" />
> "Gemini analysis: Uptrend expected due to volume spike and positive momentum indicator. Consider entry above last resistance zone."

---

## 🟧 11. Error Handling

- **Telegram not sending:** Check bot token & chat ID
- **API request failed:** Verify endpoint, credentials in HTTP node
- **Image not analyzed:** Confirm AI agent tool config
- **Workflow not triggering:** Activate workflow, check triggers

---

## 🟧 12. Security Tips

- Protect all API Keys & bot tokens in n8n credentials
- Do not expose sensitive workflow URLs in public portals
- Secure webhooks with n8n authentication if opening externally

---

## 🟧 13. Future Upgrades

- Integrate more data feeds (Yahoo Finance, Alpha Vantage)
- Add multi-user dashboard & admin controls
- PDF export of chart analysis
- Automatic periodic market reports

---

## 🟧 14. Credits

- **Developer:** Jeyaram Reddy
- **Tools:** n8n, Gemini, Telegram Bot API
- **License:** MIT

---

## ⭐ Quickstart

1. Fork & clone repo
2. Import workflow JSON in n8n
3. Set up Telegram bot and API config
4. Trigger workflow & chat with bot for instant market analysis!

---

Ready to automate your stock analysis?  
**Fork, setup, and deploy your own market agent today!**

---

## 👨‍💻 About the Developer

**Name:** Jeyaram Reddy  
**Email:** [jeyaram.reddy.ece@gmail.com](mailto:jeyaram.reddy.ece@gmail.com)  
**GitHub:** [jeyaram1023](https://github.com/jeyaram1023)  
**Portfolio:** [Click here](https://jeyaram1023.github.io/My-portfolio/)  
**Location:** India  
**Status:** Open to collaboration & freelance automation gigs!

---
---
