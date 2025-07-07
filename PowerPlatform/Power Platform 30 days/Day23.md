
# Day 23 – Power Virtual Agents & Copilot Studio: Build Your First Chatbot

---

## 📝 Overview

Power Virtual Agents (now part of Copilot Studio) allows you to build intelligent, no-code chatbots that can handle questions, trigger Power Automate flows, and connect to your business data.

In this session, you’ll build your first chatbot, define topics, add questions and responses, and connect the bot to Dataverse or a flow.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Open Copilot Studio

1. Go to [https://copilotstudio.microsoft.com](https://copilotstudio.microsoft.com)
2. Click **Start from blank** or **New bot**
3. Name your bot (e.g., `HelpDeskBot`)
4. Choose your environment and language
5. Click **Create**

---

### ✅ Step 2: Define a Topic

1. In the left menu, click **Topics**
2. Click **+ New topic**
3. Give it a name like `Submit Ticket`
4. Add **trigger phrases** (e.g., “I need help”, “report an issue”)
5. Click **Go to authoring canvas**

---

### ✅ Step 3: Build the Conversation Flow

1. Add a **message node** to greet the user
2. Add a **question node** to collect information:
   - What issue are you reporting?
   - What is your email?
3. Store responses as variables (e.g., `IssueType`, `UserEmail`)
4. Add **conditions** to branch logic if needed

---

### ✅ Step 4: Call a Power Automate Flow (Optional)

1. Add a **Call an action** node
2. Choose or create a flow that:
   - Creates a row in Dataverse or SharePoint
   - Sends an email or Teams message
3. Pass variables from the chatbot as inputs

---

### ✅ Step 5: Test and Publish Your Bot

1. Use the **Test your bot** panel to simulate conversations
2. Click **Publish > Publish this bot**
3. Share it in Teams or embed it on a website or Power Apps app

---

## 🔎 What You Should Try Today

- Create a chatbot with at least one custom topic
- Collect user input with variables
- Connect the bot to a Power Automate flow
- Test different trigger phrases and responses

---

## 🔁 Navigation

⬅️ [**Go to Day 22: Model-Driven Power Apps – structure and business logic**](/PowerPlatform/Power%20Platform%2030%20days/Day22.md)  
➡️ [**Go to Day 24: Custom Connectors – consume external APIs in Power Apps**](/PowerPlatform/Power%20Platform%2030%20days/Day24.md)
