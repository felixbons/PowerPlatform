
# Day 26 – Power BI + Power Platform: Embed Reports Into Your Apps

---

## 📝 Overview

Power BI integrates seamlessly with Power Apps and Power Automate, allowing you to visualize data, create reports, and embed interactive dashboards into your business apps. This helps users make informed decisions directly within the context of their workflows.

In this session, you’ll learn how to embed Power BI reports into Power Apps, use filters, and trigger flows based on user interaction with Power BI data.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Prepare Your Power BI Report

1. Go to [https://app.powerbi.com](https://app.powerbi.com)
2. Create or open an existing report
3. Publish it to a **workspace** (must be in **Power BI Pro** or **Premium** capacity)
4. Share access with users who will view it

---

### ✅ Step 2: Get the Report Details

1. In the workspace, click your report
2. Go to **File > Embed report > Website or portal**
3. Copy the **embed URL** (for use in Power Apps)
4. Also take note of the **report ID**, **group ID**, and **page name** if using filters

---

### ✅ Step 3: Embed Power BI in Power Apps

1. Go to [https://make.powerapps.com](https://make.powerapps.com)
2. Open or create a Canvas app
3. Insert the **Power BI tile** control:
   - **Insert > Charts > Power BI tile**
4. Select:
   - Workspace
   - Dashboard
   - Tile

> 💡 *If you need more flexibility, use the Power BI JavaScript SDK or embed via iframe in Power Pages.*

---

### ✅ Step 4: Add Filters and Context

1. In Power BI, create a **report page filter** (e.g., `EmployeeID = LoggedInUser`)
2. Use **PowerApps filters** to pass context to Power BI via query string
3. Advanced: Use **Power BI Embedded (Azure)** for secure user-level embedding

---

### ✅ Step 5: Trigger Flows from Power BI Insights

1. Create a **button or KPI** in Power BI
2. Use Power Automate visual (in Power BI):
   - Add the **Power Automate for Power BI** visual
   - Configure the flow to receive inputs from the report
   - Perform actions like sending emails, updating records, or alerts

---

## 🔎 What You Should Try Today

- Embed a Power BI tile into a Power App
- Add filters to tailor the visual to the user
- Add a Power Automate visual in Power BI and trigger a flow
- Explore embedding entire reports into portals or model-driven apps

---

## 🔁 Navigation

⬅️ [**Go to Day 25: PDF generation, emails, and attachments using Power Automate**](/PowerPlatform/Power%20Platform%2030%20days/Day25.md)  
➡️ [**Go to Day 27: Solutions, environments, export/import practices**](/PowerPlatform/Power%20Platform%2030%20days/Day27.md)
