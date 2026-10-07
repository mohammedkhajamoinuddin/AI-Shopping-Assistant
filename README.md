# 🛍️ AI Shopping Assistant

An AI-powered shopping assistant built using **n8n, Telegram, and Google Gemini** that helps users discover Amazon products through natural-language queries. The assistant searches for relevant products and delivers recommendations directly in Telegram.

## 📌 Overview

Online shopping can be overwhelming due to the number of products available, the time required to compare options, and the difficulty of finding products within a budget.

This project uses an AI agent and an automated n8n workflow to simplify product discovery through a conversational Telegram bot.

## ✨ Features

- **Text-Based Product Search:** Search for products using natural-language requests, such as "running shoes under ₹5,000".
- **AI-Powered Assistance:** Uses an AI agent to interpret shopping queries.
- **Amazon Product Search:** Integrates with a scraper API to retrieve product information.
- **Telegram Integration:** Receive shopping recommendations directly in Telegram.
- **Automated Workflow:** Connects messaging, AI processing, product search, and response delivery using n8n.

## 🏗️ Architecture

The workflow follows this sequence:

1. **Telegram Trigger** — receives the user's message.
2. **AI Agent** — interprets the shopping request.
3. **Product Search Tool** — retrieves relevant Amazon product information through the configured scraper API.
4. **AI Response Generation** — organizes the retrieved information into a readable response.
5. **Telegram Response** — sends the recommendations back to the user.

## 📸 Screenshots

### 1. Telegram Shopping Assistant

The user sends a shopping query through Telegram and receives a response from the assistant.

![Telegram Shopping Assistant](screenshots/00-telegram-chat.png)

![Telegram Shopping Assistant - Response](screenshots/01-telegram-chat.png)

### 2. n8n Workflow

The n8n workflow connects the Telegram trigger, AI agent, product search, and response nodes.

![n8n Workflow](screenshots/02-n8n-workflow.png)

### 3. AI Agent Configuration

The AI agent processes shopping queries and uses the configured tools to generate relevant recommendations.

![AI Agent Configuration](screenshots/03-ai-agent.png)

## 🧰 Tech Stack

- **Workflow Automation:** n8n
- **Conversational Interface:** Telegram Bot API
- **AI Model:** Google Gemini
- **Product Discovery:** Amazon product scraper API
- **Integration:** n8n HTTP Request and AI Agent nodes

## ⚙️ Setup

### Prerequisites

- An n8n instance
- A Telegram bot created using [BotFather](https://t.me/BotFather)
- Google Gemini API credentials
- Access to the configured Amazon product scraper API

### Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/mohammedkhajamoinuddin/AI-Shopping-Assistant.git
   ```

2. Open your n8n instance.
3. Import `Ai-Shopping-Assistant-Workflow.json`.
4. Configure the required Telegram, AI model, and scraper API credentials in n8n.
5. Verify the product search endpoint and its request parameters.
6. Activate the workflow and send a shopping query to your Telegram bot.

**Security:** Never commit API keys, bot tokens, passwords, or other credentials to GitHub. Configure credentials securely within n8n.

## 🎯 Example Use Case

**User:** Find running shoes under ₹5,000.

**Assistant:** Searches for relevant products and returns available product details, such as names, prices, and ratings, when provided by the scraper.

## 🚀 Future Enhancements

- Voice-based shopping queries
- Personalized fashion and styling recommendations
- Product comparisons based on price and ratings
- Improved product filtering and recommendation relevance

## 👨‍💻 Author

**Mohammed Khaja Moinuddin**

- GitHub: [mohammedkhajamoinuddin](https://github.com/mohammedkhajamoinuddin)
- LinkedIn: [Mohammed Khaja Moinuddin](https://www.linkedin.com/in/mohammed-khaja-moinuddin05/)

---

⭐ If you find this project interesting, consider giving the repository a star.
