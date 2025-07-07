# Day 5 – Connectors: What They Are and How They Work (SharePoint, Excel, Dataverse)

---

## 📝 Overview

Connectors in Power Platform are the bridge between your app and external or internal data sources. With over 900 connectors available, Power Apps and Power Automate can connect to services like **SharePoint**, **Excel**, **Dataverse**, SQL, Outlook, and many more.

In this session, you’ll learn how connectors work, when to use each, and how to set up the most commonly used ones — SharePoint, Excel, and Dataverse.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Understand the Types of Connectors

- **Standard connectors**: Free to use (e.g., SharePoint, Excel, Outlook)
- **Premium connectors**: Require a license (e.g., SQL Server, Dataverse, Salesforce)
- **Custom connectors**: Built by you to connect with external APIs

---

### ✅ Step 2: Add a SharePoint Connector

1. In [https://make.powerapps.com](https://make.powerapps.com), open an existing or new **Canvas app**
2. Click **Data** (left panel)
3. Click **+ Add data**
4. Search for **SharePoint** and click it
5. Sign in with your credentials
6. Enter your site URL and select a list (e.g., `Requests`, `Employees`)
7. The list is now connected to your app and visible in the data pane

---

### ✅ Step 3: Add an Excel Connector (Stored in OneDrive)

1. From the **Data** panel, click **+ Add data**
2. Search for **Excel Online (Business)** or **OneDrive for Business**
3. Sign in to your OneDrive account
4. Navigate to your Excel file (ensure it has **formatted tables**)
5. Select the table(s) you want to use
6. Now you can use it with galleries, forms, and dropdowns

---

### ✅ Step 4: Connect to Dataverse Tables

1. From **make.powerapps.com**, go to **Tables** under Dataverse
2. Use a built-in table (e.g., `Contact`) or create your own
3. In a Canvas app, open **Data** and add **Dataverse**
4. Choose the tables you want to use
5. Dataverse allows you to model complex relationships and secure your data

---

### ✅ Step 5: Use Connected Data in Your App

- Use **Gallery.Items = [YourDataSource]** to show data
- Use **Form.DataSource = [YourDataSource]** to edit records
- Use functions like **Patch**, **Collect**, **LookUp**, and **Filter** to interact with data

---

## 🔎 What You Should Try Today

- Connect a SharePoint list to a Canvas app
- Create a small Excel table and connect it to an app
- Browse Dataverse tables and connect one to a new app
- Explore how each data source behaves (delegation, speed, formatting)

---

## 🔁 Navigation

⬅️ [**Go to Day 4: Build your first Canvas app from a template**](/PowerPlatform/Power%20Platform%2030%20days/Day04.md)  
➡️ [**Go to Day 6: Introduction to Power Automate – Your first automated flow**](/PowerPlatform/Power%20Platform%2030%20days/Day06.md)
