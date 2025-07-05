# 🚀 N8N Lead Scoring & Automation Workflow

## 📌 Project Overview

This project demonstrates an automated **lead scoring and notification system** built entirely in **n8n**, created for the REMWaste technical challenge (n8n Expert role). It simulates a real-world workflow that:

- Captures incoming leads (form submission / Webhook)
- Scores each lead based on custom logic (budget + interest)
- Stores Leads in Airtable
- Sends alerts via Slack for high-priority leads
- Creates calendar invites and follow-up emails for Hot leads

---

## ⚙️ Workflow Features

| Feature                      | Status |
|-----------------------------|--------|
| Custom scoring logic        | ✅     |
| Slack notification (Hot)    | ✅     |
| Airtable integration        | ✅     |
| Google Calendar invite      | ✅     |
| Delay-based email follow-up | ✅     |
| API-based lead parsing      | ✅     |

---

## 🧠 Lead Scoring Logic

The lead is scored using the following custom criteria:

| Condition                            | Score   |
|-------------------------------------|---------|
| Budget ≥ £5000 & Interest = High    | 🔥 Hot  |
| Budget ≥ £3000 & Interest = Medium  | ☄️ Warm |
| Else                                | ❄️ Cold |

Only **Hot leads** trigger the Slack message and follow-up.

---

## 🗂️ Airtable Fields

- full_name  
- email  
- budget  
- interest_level  
- lead_score  
- createdTime  

---

## 🛠️ Tools & Services Used

- [n8n Cloud](https://n8n.io/)
- [Airtable](https://airtable.com)
- [Slack Webhooks](https://api.slack.com/messaging/webhooks)
- [Google Calendar](https://calendar.google.com)
- Groq API (Chat Memory node)

---

## 🧪 How to Use This Workflow

1. Clone this repo or download the `.json` file from the `/export/` folder.
2. In **N8N**, go to **Settings → Import from File**.
3. Paste your own:
   - Airtable API key + Base ID
   - Slack Webhook URL
   - Google Calendar credentials
4. Execute the workflow or trigger via webhook to test.

---

## 📈 Hypothetical Impact — Example Business

**ZentraConsulting Ltd** (fictional) uses this workflow to qualify clients:

| Stage            | Leads/Month | Conversion Rate |
|------------------|-------------|-----------------|
| Captured         | 300         | -               |
| Warm Qualified   | 180         | 60%             |
| Hot Leads        | 90          | 30%             |
| Converted Clients| 36          | 40%             |

> 🧮 36 × £1200 average spend = **£43,200/month**

---

## 📦 File Structure


---

## 👤 Author

**Banele Mlalazi**  
Automation & Workflow Specialist  
[LinkedIn](https://linkedin.com/in/banelemlalazi) | [Email](mailto:banelemlalazi@gmail.com)

---

> 📝 *This repository contains a demonstration project. All business names and data are fictional and used only for illustrative purposes.*


