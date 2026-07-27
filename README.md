# Customer Feedback Automation using n8n

## Overview

This project automates customer feedback management using n8n.

The workflow classifies customer feedback into:
- Complaint
- Compliment
- Feature Addition Request

Based on the classification, the workflow:
- Stores the feedback in Airtable
- Sends a Telegram notification
- Sends an acknowledgment email to the customer

---

## Technologies Used

- n8n
- Groq LLM
- Airtable
- Gmail API
- Telegram Bot API

---

## Workflow

1. Customer submits the form.
2. AI classifies the feedback.
3. Switch node routes it.
4. Data is stored in Airtable.
5. Telegram notification is sent.
6. Customer receives an email acknowledgment.

---

## Features

- AI-powered feedback classification
- Automated database storage
- Telegram alerts
- Personalized email responses
- No manual intervention

---

## Screenshots

(Add screenshots here)

---

## Installation

1. Clone the repository.
2. Import `workflow.json` into n8n.
3. Configure:
   - Airtable API
   - Telegram Bot
   - Gmail
   - Groq API Key
4. Run the workflow.

---

## Author

Akshat Vishnoi
