
# Day 18 – Introduction to Dataverse: Structure, Tables, and Relationships

---

## 📝 Overview

Dataverse is Microsoft’s secure, scalable, and relational data platform integrated into Power Platform. It allows you to define data structures using **tables**, **columns**, and **relationships**, similar to a traditional database — but with a low-code interface.

Today you'll explore Dataverse’s core concepts, create a custom table, define columns, and understand relationships between tables.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Access Dataverse in Maker Portal

1. Go to [https://make.powerapps.com](https://make.powerapps.com)
2. In the left panel, click **Tables**
3. You’ll see a list of **standard**, **custom**, and **virtual** tables
4. Click **+ New table**

---

### ✅ Step 2: Create a Custom Table

1. Name your table (e.g., `Project`)
2. Add a **Display Name**, **Plural Name**, and optional description
3. Keep **Enable attachments** unchecked (optional)
4. Click **Save**

---

### ✅ Step 3: Add Custom Columns

1. After saving the table, go to the **Columns** tab
2. Click **+ Add column**
3. Choose:
   - **Name**: `ProjectStatus`
   - **Data type**: Choice or Text
4. Repeat for other fields like:
   - `StartDate` (Date)
   - `Budget` (Currency)
   - `ClientEmail` (Text)
5. Save your changes

---

### ✅ Step 4: Understand Primary Key and Alternate Keys

- Every Dataverse table has an internal **Primary Key (GUID)** and **Primary Name column**
- You can define **Alternate Keys** for indexing and duplicate detection (e.g., `ProjectCode`)

---

### ✅ Step 5: Create Relationships Between Tables

1. Open your `Project` table > Go to **Relationships**
2. Click **+ New relationship**
3. Choose relationship type:
   - **1:N (One-to-Many)**: One client → many projects
   - **N:1 (Many-to-One)**: Many tasks → one project
   - **N:N (Many-to-Many)**: Many users assigned to many tasks
4. Select target table (e.g., `Client`)
5. Name the relationship and click **Done**

---

## 🔎 What You Should Try Today

- Create a table with at least 3 custom columns
- Add a One-to-Many relationship to another table
- Explore table views, forms, and dashboards from the table's menu
- Consider how you would model real-world entities (e.g., Employees, Projects, Requests)

---

## 🔁 Navigation

⬅️ [**Go to Day 17: Advanced use of expressions and error handling**](/PowerPlatform/Power%20Platform%2030%20days/Day17.md)  
➡️ [**Go to Day 19: Creating and using custom tables in Dataverse**](/PowerPlatform/Power%20Platform%2030%20days/Day19.md)
