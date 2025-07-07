
# Day 19 – Creating and Using Custom Tables in Dataverse

---

## 📝 Overview

Custom tables in Dataverse allow you to model the unique data structure of your business applications. With customizable columns, relationships, and views, you can build powerful low-code data layers for your apps and flows.

In this session, you'll learn how to create a custom table from scratch, customize it with business columns, add relationships, and use it in Power Apps and Power Automate.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Create a Custom Table

1. Go to [https://make.powerapps.com](https://make.powerapps.com)
2. In the left panel, click **Tables > + New table**
3. Provide:
   - **Display Name**: `Ticket`
   - **Plural Name**: `Tickets`
   - Enable or disable attachments and notes as needed
4. Click **Create**

---

### ✅ Step 2: Add Custom Columns

1. Open the `Ticket` table
2. Go to the **Columns** tab > **+ Add column**
3. Add relevant fields such as:
   - `Title` (Text)
   - `Category` (Choice)
   - `UrgencyLevel` (Choice or Number)
   - `ReportedDate` (Date)
   - `Status` (Choice)
4. Define business rules or default values as needed

---

### ✅ Step 3: Create Relationships

1. Open the **Relationships** tab > **+ New relationship**
2. Choose the type (e.g., **N:1** from Ticket to Employee)
3. Select the related table (e.g., `Employee`)
4. Name and save the relationship

---

### ✅ Step 4: Create Views and Forms

1. Go to the **Views** tab
2. Modify or create a public view (e.g., `Active Tickets`)
3. Select columns to show and set filters/sorting
4. Switch to the **Forms** tab
5. Edit or design a form layout for creating and editing tickets

---

### ✅ Step 5: Use the Table in an App or Flow

**In Power Apps:**
1. Create a new Canvas or Model-driven app
2. Add the `Ticket` table as a data source
3. Use galleries and forms to display or edit ticket data

**In Power Automate:**
1. Use actions like:
   - `Add a new row`
   - `Get a row by ID`
   - `Update a row`
2. Connect logic based on ticket `Status`, `Urgency`, or `Category`

---

## 🔎 What You Should Try Today

- Create a custom table with at least 5 fields
- Set up a relationship with another table
- Customize a view and a form layout
- Use the custom table in a Canvas app or an automated flow

---

## 🔁 Navigation

⬅️ [**Go to Day 18: Introduction to Dataverse – structure, tables, and relationships**](/PowerPlatform/Power%20Platform%2030%20days/Day18.md)  
➡️ [**Go to Day 20: Power Automate + Dataverse – build connected flows**](/PowerPlatform/Power%20Platform%2030%20days/Day20.md)
