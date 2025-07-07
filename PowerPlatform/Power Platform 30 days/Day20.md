
# Day 20 – Power Automate + Dataverse: Build Connected Flows

---

## 📝 Overview

Dataverse and Power Automate work together seamlessly, allowing you to automate business processes based on data stored in Dataverse. You can trigger flows when rows are added or modified, and perform actions like creating, updating, or deleting rows across related tables.

In this session, you’ll create a flow triggered by changes in a Dataverse table, automate responses, and learn how to integrate data-driven logic into your workflows.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Create a Trigger Based on Dataverse

1. Go to [https://make.powerautomate.com](https://make.powerautomate.com)
2. Click **Create > Automated cloud flow**
3. Set a name like `NotifyNewTicket`
4. Choose the trigger:  
   `When a row is added, modified or deleted`
5. Click **Create**

---

### ✅ Step 2: Configure the Trigger

1. Choose:
   - **Change type**: `Added` or `Modified`
   - **Table name**: `Tickets` (or your custom table)
   - **Scope**: Organization or User
2. Click **+ New step** to continue

---

### ✅ Step 3: Add Conditions and Logic

1. Add a **Condition**:
   ```text
   Status equals "Open"
   ```
2. In the **If yes** branch, add an action like:
   - Send email to support team
   - Post a message to Microsoft Teams
   - Update another table row

---

### ✅ Step 4: Create a Record in Another Table

1. Add an action: `Add a new row`
2. Choose the related table (e.g., `TicketLog`)
3. Map fields using dynamic content from the trigger:
   ```text
   Ticket ID = Row ID
   Action = "Created"
   Timestamp = utcNow()
   ```

---

### ✅ Step 5: Test and Monitor the Flow

1. Save and **Test** the flow manually or automatically
2. Add or edit a row in your Dataverse table
3. Go to **My Flows > Run history** to check success/fail
4. Adjust logic as needed

---

## 🔎 What You Should Try Today

- Trigger a flow from a new Dataverse row
- Add a condition and branch logic
- Create a row in a related table based on the trigger
- Explore other Dataverse actions like `Get a row`, `Update a row`

---

## 🔁 Navigation

⬅️ [**Go to Day 19: Creating and using custom tables in Dataverse**](/PowerPlatform/Power%20Platform%2030%20days/Day19.md)  
➡️ [**Go to Day 21: Dataverse security – roles, permissions, and column-level security**](/PowerPlatform/Power%20Platform%2030%20days/Day21.md)
