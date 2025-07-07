
# Day 22 – Model-Driven Power Apps: Structure and Business Logic

---

## 📝 Overview

Model-driven apps are based on your data model in Dataverse and automatically generate user interfaces that are responsive and accessible. Unlike canvas apps, model-driven apps emphasize **data structure, business rules**, and **relationships**, making them ideal for enterprise-grade solutions.

Today you’ll create a model-driven app, define navigation, and configure views, forms, and business logic like rules and calculated fields.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Create a Model-Driven App

1. Go to [https://make.powerapps.com](https://make.powerapps.com)
2. Click **Apps > + New app > Model-driven app**
3. Choose **Modern App Designer**
4. Name your app (e.g., `Project Tracker`)
5. Click **Create**

---

### ✅ Step 2: Add Tables to Your App

1. In the app designer, click **+ Add page**
2. Select **Dataverse table** and choose one or more tables (e.g., `Project`, `Employee`)
3. These will appear in the left-side navigation of your app
4. Reorder and rename pages as needed

---

### ✅ Step 3: Configure Views and Forms

1. Click on a table to open **View** settings
2. Select or create custom views (e.g., Active Projects)
3. Go to **Forms** and customize the layout:
   - Tabs, columns, sections
   - Read-only fields
   - Header controls

---

### ✅ Step 4: Add Business Rules

1. Open a table > Go to **Business rules**
2. Click **+ Add business rule**
3. Add conditions and actions (e.g., if `Status = Closed`, then `CompletionDate` is required)
4. Activate the rule when done

---

### ✅ Step 5: Use Calculated or Rollup Fields

1. Go to the **Columns** tab in a table
2. Create a new column or edit an existing one
3. Choose:
   - **Calculated field**: use formulas like `Budget - Cost`
   - **Rollup field**: aggregate data from related records
4. Save and publish

---

### ✅ Step 6: Preview and Share Your App

1. In the app designer, click **Play** to preview
2. Test navigation, views, and forms
3. Save and **Publish** the app
4. Share it with users under **File > Share**

---

## 🔎 What You Should Try Today

- Create a model-driven app with at least 2 tables
- Customize one view and one form
- Add a business rule to enforce logic
- Create a calculated or rollup column

---

## 🔁 Navigation

⬅️ [**Go to Day 21: Dataverse security – roles, permissions, and column-level security**](/PowerPlatform/Power%20Platform%2030%20days/Day21.md)  
➡️ [**Go to Day 23: Power Virtual Agents & Copilot Studio – build your first chatbot**](/PowerPlatform/Power%20Platform%2030%20days/Day23.md)
