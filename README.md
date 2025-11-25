


AI Cold Email Automation (n8n Workflow)

This repository contains an automated cold-email workflow built using n8n, Google Sheets, OpenAI, and Gmail.
It reads contacts from a Google Sheet, generates AI-written personalized emails, sends them via Gmail, and updates the sheet with status + timestamps.

🚀 Features

* Read HR contact data from Google Sheets
* Generate personalized cold emails with OpenAI
* Send emails automatically via Gmail
* Update Sheet with status (`Sent`) and timestamp
* Fully customizable prompt, subject, and email tone

🧩 Workflow Steps

1. Manual Trigger
2. Get row(s) from Google Sheet
3. Generate email using OpenAI (Message a Model)
4. Send email via Gmail
5. Update sheet (Status + Last email sent at)

📄 Google Sheet Format

Your Google Sheet should contain:

| Name | Email | Status | Last email sent at | Note |

Email is required.
Status and Last email sent at are automatically updated.


🛠 Setup

1. Import the Workflow

Open n8n → Workflows → Import
Upload the provided .json file

2. Add Credentials

You’ll need to configure:

Google Sheets OAuth
Gmail OAuth
OpenAI API Key


3. Update Sheet & Prompt

Inside the workflow:

Set your Google Sheet
Customize the prompt in the OpenAI node if needed

Run the workflow → emails will be generated + sent → sheet updates automatically.

📦 Future Extensions

You can add:

Automated follow-ups after 2–3 days
Reply detection
Webhook trigger for external frontend
Multi-user Gmail authentication

👩‍💻 Author

Muskan Gupta
LinkedIn:https://www.linkedin.com/in/muskan-gupta98/



