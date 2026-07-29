# AI Commercial Proposal Generator & Auditor (n8n + Actor-Critic Pattern)

Enterprise-grade architecture for automated B2B commercial proposal (КП) generation. Built with n8n and Python, this system uses the Actor-Critic LLM pattern to write, ruthlessly critique, and rewrite proposals without human intervention.

## How it works (Architecture)
Unlike basic ChatGPT wrappers that generate generic and watered-down texts, this system utilizes a multi-agent validation process:

1. **Agent 1 (Draftsman):** Ingests the client brief and generates an initial proposal draft.
2. **Agent 2 (The Critic):** Acts as a strict Commercial Director. It analyzes the draft for clichés, lack of ROI metrics, and poor structure, outputting a strict error log.
3. **Agent 3 (Copywriter):** Rewrites the final proposal based on the Critic's feedback.
4. **Delivery:** The polished, high-converting proposal is sent directly to Telegram or CRM.

## Video Demonstration (Proof of Work)
Watch the full breakdown of the logic, prompts, and architecture in action:
https://youtu.be/vOW1qQjSYGc

## Commercial License & Source Code
This repository serves as architectural documentation. 

The complete, production-ready **n8n JSON workflows** and **system prompts** are available under a commercial license. You can purchase the source code "as-is" and deploy it on your servers immediately.

[Get the Full Source Code on Kwork](https://kwork.ru/script-programming/53800637/arkhitektura-ii-kontrolya-otdela-prodazh-analiz-dialogov)

### Tech Stack
* **Orchestration:** n8n
* **Logic Framework:** Actor-Critic Multi-Agent Pattern
* **AI/LLM:** DeepSeek V3 / GPT-4o / Claude 4.0
* **Integration:** Telegram API, Webhooks

---
*Developed by a Senior B2B Automation Engineer.* 
*For custom architecture design, contact me via Telegram: https://t.me/chernyaevi*
