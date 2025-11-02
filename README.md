# AI Email Manager — n8n Workflow

**Project:** AI Email Manager  
**Author:** Lokesh Ram  
**Buildathon:** OpenAI × NxtWave Buildathon 2025  

---

## **Project Overview**

The **AI Email Manager** is an intelligent workflow automation built using **n8n** and **OpenAI** that helps users manage Gmail inboxes efficiently.  
It uses AI to classify emails and performs automated actions such as marking emails as read/unread, sending auto-replies, and scheduling events in Google Calendar.

**Key Features:**
- **AI Classification:** Uses OpenAI GPT-4o-mini to classify emails as important or unimportant.
- **Automated Actions:**
  - Important emails → Keep unread + schedule event in Google Calendar.
  - Unimportant emails → Mark as read + send auto-reply.
- **Analytics:** Logs summary of processed emails (important vs unimportant).
- **Integration:** Works with Gmail API, Google Calendar API, and OpenAI.
- **Secure:** Google OAuth2 authentication ensures credentials are never shared.

---

## **Workflow Architecture**

