# 🤖 AI Customer Feedback Automation using n8n

An intelligent no-code workflow built with **n8n** that automatically classifies customer feedback using **Groq AI**, stores it in **Airtable**, sends **Telegram notifications**, and emails personalized acknowledgements to customers.

---

## 🚀 Features

- 📝 Accepts customer feedback through an n8n Form.
- 🤖 Uses **Groq LLM** to classify feedback into:
  - Complaint
  - Compliment
  - Feature Addition Request
- 🔀 Automatically routes feedback using a **Switch** node.
- 📊 Stores categorized feedback in separate Airtable tables.
- 📲 Sends instant Telegram notifications to the administrator.
- 📧 Sends personalized acknowledgement emails to customers.
- ⚡ Fully automated workflow with no manual intervention.

---

## 🛠️ Tech Stack

- **n8n**
- **Groq API (LLM)**
- **Airtable**
- **Telegram Bot API**
- **Gmail**
- AI Agent
- Switch Node
- Merge Node

---

## 📋 Workflow

```
Customer Form
      │
      ▼
 AI Agent (Groq)
      │
      ▼
    Merge Node
      │
      ▼
   Switch Node
      │
 ┌────┼────┐
 │    │    │
 ▼    ▼    ▼
Complaint  Compliment  Feature Request
 │          │             │
 ▼          ▼             ▼
Airtable Airtable Airtable
 │          │             │
 ▼          ▼             ▼
Telegram Telegram Telegram
 │          │             │
 ▼          ▼             ▼
 Gmail     Gmail       Gmail
```

---

## 📷 Workflow Screenshot

> Add your workflow screenshot inside a folder named `screenshots`.

```text
screenshots/workflow.png
```

Example:

![Workflow](screenshots/workflow.png)

---

## 📂 Project Structure

```
Customer-Feedback-Automation
│
├── workflow.json
├── README.md
├── LICENSE
└── screenshots
    └── workflow.png
```

---

## 📊 Airtable Tables

The workflow stores records in three separate Airtable tables:

- Complaint
- Compliment
- Feature Addition Request

Each record contains:

- Full Name
- Email
- Feedback
- Category

---

## 📲 Telegram Notification

Whenever a customer submits feedback, the administrator instantly receives a Telegram notification.

Example:

```
🚨 Customer Complaint

👤 Name: Rahul Sharma

📝 Feedback:
The application crashes while uploading files.
```

---

## 📧 Customer Acknowledgement

Customers automatically receive an acknowledgement email based on the feedback category.

### Complaint

- Confirmation that the complaint has been received.
- Assurance that the support team will review it.

### Compliment

- Thank-you message for the positive feedback.

### Feature Addition Request

- Confirmation that the suggestion has been forwarded to the product team.

---

## ⚙️ Installation

1. Clone this repository.

```bash
git clone https://github.com/AKSHATV25/Customer-Feedback-Automation.git
```

2. Import `workflow.json` into n8n.

3. Configure your credentials:

- Groq API
- Airtable
- Telegram Bot
- Gmail

4. Activate the workflow.

---

## 📈 Future Improvements

- Slack Integration
- Microsoft Teams Notifications
- Dashboard & Analytics
- Weekly Email Reports
- Sentiment Score
- Multi-language Support

---

## 👨‍💻 Author

**Akshat Vishnoi**

B.Tech CSE (AI & ML)

GitHub: https://github.com/AKSHATV25

---

## ⭐ If you like this project

Give this repository a ⭐ on GitHub!
