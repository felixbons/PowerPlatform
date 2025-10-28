
# Day 15 – Power Automate: Creating Automated, Instant, and Scheduled Flows

---

## 📝 Overview

Power Automate supports three types of flows:
- **Automated flows**: Triggered by events like receiving an email or adding a SharePoint item.
- **Instant flows**: Triggered manually via a button in Power Apps or from the Power Automate app.
- **Scheduled flows**: Run at specific times or intervals (e.g., every day at 8 AM).

In this session, you'll learn how to create each type of flow and understand their common use cases.

![Step 1](/PowerPlatform/assets/PowerPlatform30days/Day15/Day15_1.png)
---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Create an Automated Flow

1. Go to [https://make.powerautomate.com](https://make.powerautomate.com)
2. Click **Create > Automated cloud flow**
3. Enter a name (e.g., `NotifyOnNewItem`)
4. Choose a trigger, such as **When an item is created (SharePoint)** or **When a new email arrives**
5. Click **Create**
6. Add an action, e.g.:
   ```powerfx
   Send an email (V2)
   ```
7. Save and test the flow

![Automated Flow](/PowerPlatform/assets/PowerPlatform30days/Day15/Day15_2.png)

---

### ✅ Step 2: Create an Instant Flow

1. From the **Create** menu, choose **Instant cloud flow**
2. Choose **Manually trigger a flow**
3. Add an action like:
   ```powerfx
   Post a message in Microsoft Teams
   ```
4. Save the flow
5. Run it manually from **My Flows** or from the **Power Automate mobile app**

![Instant Flow](/PowerPlatform/assets/PowerPlatform30days/Day15/Day15_3.png)

---

### ✅ Step 3: Create a Scheduled Flow

1. Click **Create > Scheduled cloud flow**
2. Set:
   - Flow name
   - Start time
   - Frequency (e.g., daily, weekly, every 15 minutes)
3. Click **Create**
4. Add actions such as:
   - Run a report
   - Send summary emails
   - Clean up records
5. Save and monitor the run history

![Schedule flow](/PowerPlatform/assets/PowerPlatform30days/Day15/Day15_4.png)

---

### ✅ Step 4: Monitor and Edit Flows

1. Go to **My Flows**
2. Click on a flow to:
   - View run history
   - Check for errors
   - Edit or turn off the flow

![Monitor and edit flows](/PowerPlatform/assets/PowerPlatform30days/Day15/Day15_5.png)

---

## 🔎 What You Should Try Today

- Create one of each flow type (automated, instant, scheduled)
- Test each and check the run logs
- Modify one flow to include two or more actions
- Try a trigger with dynamic content (e.g., use email subject in a Teams post)

---

## 🔁 Navigation

⬅️ [**Go to Day 14: Publishing, sharing, and permissions in a Canvas app**](/PowerPlatform/Power%20Platform%2030%20days/Day14.md)  
➡️ [**Go to Day 16: Variables, conditions, and loops in Power Automate**](/PowerPlatform/Power%20Platform%2030%20days/Day16.md)
