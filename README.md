# AI Email Manager - n8n Workflow

## Project Overview
AI Email Manager is an intelligent email automation workflow built using n8n and OpenAI. It reads emails from your Gmail inbox, classifies them as important or unimportant using an AI agent, and performs smart actions automatically.

- Important emails: Keep unread and schedule events in Google Calendar.
- Unimportant emails: Mark as read and send an auto-reply.

This workflow helps users manage emails efficiently, prioritize important messages, and automate responses to unimportant emails.

## Features
- AI-powered email classification using GPT-4o-mini.
- Automatic handling of important and unimportant emails.
- Integration with Gmail for reading and sending emails.
- Integration with Google Calendar for scheduling follow-ups.
- Analytics summary of processed emails.

## Technology Stack
- **n8n**: No-code workflow automation platform.
- **OpenAI GPT-4o-mini**: Classify email importance and extract event information.
- **Gmail API**: Read, mark as read, and auto-reply to emails.
- **Google Calendar API**: Schedule events for important emails.

## Setup Instructions
1. Export the workflow JSON file (`Email Manager Enhanced.json`) from this repository.
2. Import the workflow into your n8n instance (cloud or self-hosted).
3. Connect your Gmail account using OAuth2 credentials in n8n.
4. Connect your Google Calendar account using OAuth2 credentials in n8n.
5. Activate the workflow. Emails will be processed automatically as per the workflow logic.

## Workflow Structure
1. **Gmail Trigger**: Monitors incoming emails in your inbox.
2. **AI Agent**: Uses OpenAI GPT model to classify emails and extract event information.
3. **Parse AI Output**: Processes AI response and extracts importance, category, event date, and event time.
4. **If Important**: Routes emails based on importance.
   - **Important** → Google Calendar event.
   - **Unimportant** → Mark as read and send auto-reply.
5. **Analytics Summary**: Generates a summary of processed emails.

## Usage
Once the workflow is active:
- Incoming emails will be automatically classified.
- Important emails will appear in Google Calendar.
- Unimportant emails will receive an auto-reply and be marked as read.
- Analytics summary can be viewed in the workflow logs.

## Authors
- Lokesh Ram

## License
This project is licensed under MIT License.
