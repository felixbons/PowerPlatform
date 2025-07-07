# Day 6 – Introduction to Power Automate – Your First Automated Flow

---

## 📝 Overview

Power Automate allows you to create automated workflows between your favorite apps and services to synchronize files, get notifications, collect data, and more — all without writing code.

In this session, you’ll create your first **automated cloud flow**, triggered by a simple event like receiving an email or submitting a form. You'll also explore how to find templates and understand the basic flow structure.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Open Power Automate

- Go to [https://make.powerautomate.com](https://make.powerautomate.com)
- Make sure you're in the correct **environment** (top-right dropdown)

---

### ✅ Step 2: Create a New Automated Flow

1. On the left panel, click **Create**
2. Select **Automated cloud flow**
3. Enter a **name** (e.g., `NotifyOnNewEmail`)
4. Search for a trigger (e.g., **When a new email arrives (V3)**)
5. Choose the Outlook connection
6. Click **Create**

---

### ✅ Step 3: Add an Action

1. After the trigger is set, click **+ New step**
2. Search for **Send me a mobile notification** or **Send an email (V2)**
3. Fill in the required fields (e.g., email subject, body)
4. Use dynamic content like `From`, `Subject`, or `Body` from the email trigger

---

### ✅ Step 4: Save and Test the Flow

- Click **Save** at the bottom right
- Click **Test** > **Manually**
- Perform the trigger action (e.g., send yourself an email)
- Wait for the flow to run and check the result in the **Run history**

---

### ✅ Step 5: Explore Flow Templates

- Go back to the **Create** tab
- Scroll down and explore **pre-built templates**
- Try out examples like:
  - Save email attachments to OneDrive
  - Post a Teams message when a SharePoint item is created

---

## 🔎 What You Should Try Today

- Build a basic flow triggered by a new email
- Add a second action to send a notification or Teams message
- Explore and run a template flow
- Check your flow run history and understand success/error logs

---

## 🔁 Navigation

⬅️ [**Go to Day 5: Connectors – What they are and how they work (SharePoint, Excel, Dataverse)**](/PowerPlatform/Power%20Platform%2030%20days/Day05.md)  
➡️ [**Go to Day 7: Best practices for working with the Power Platform interface**](/PowerPlatform/Power%20Platform%2030%20days/Day07.md)
