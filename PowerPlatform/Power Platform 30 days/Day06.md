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
![Create Flow](/PowerPlatform/assets/PowerPlatform30days/Day6/Step2.png)

---

### ✅ Step 3: Add an Action

1. After the trigger is set, click **+ New step**
2. Search for **Create item**
3. Select SharePoint Option **Create item**
![Create Flow](/PowerPlatform/assets/PowerPlatform30days/Day6/Step3_1.png)
3. Select the SPO site and the List
4. Add title `Filled from flow` 
![Create Flow](/PowerPlatform/assets/PowerPlatform30days/Day6/Step3_2.png)

---

### ✅ Step 4: Save and Test the Flow

- Click **Save** at the bottom right
![Create Flow](/PowerPlatform/assets/PowerPlatform30days/Day6/Step4_1.png)
- Click **Test** > **Manually**
![Create Flow](/PowerPlatform/assets/PowerPlatform30days/Day6/Step4_2.png)
- Wait for the flow to run and check the result in the **Run history**
- Confimr in your SharePoint list that you have a new record.
---

### ✅ Step 5: Explore Flow Templates

- Go back to the **Create** tab
- Scroll down and explore **pre-built templates**
- Try out examples like:
  - Save email attachments to OneDrive
  - Post a Teams message when a SharePoint item is created
![Templates](/PowerPlatform/assets/PowerPlatform30days/Day6/Step5.png)
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
