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

[List of all Standard tier connectors](https://learn.microsoft.com/en-us/connectors/connector-reference/connector-reference-standard-connectors)
---

### ✅ Step 2: Add a SharePoint Connector

1. In [https://make.powerapps.com](https://make.powerapps.com), open an existing or new **Canvas app**, [if you have questions, plase follow points 1 nad 2 from Day 4](https://github.com/felixbons/PowerPlatform/blob/main/PowerPlatform/Power%20Platform%2030%20days/Day04.md#-step-1-open-power-apps-maker-portal)
2. Click **Data** (left panel)
3. Click **+ Add data**
![Data and Add Data](/PowerPlatform/assets/PowerPlatform30days/Day5/Step1/2and3.png)
4. Search for **SharePoint** and click it
![Search for SharePoint](/PowerPlatform/assets/PowerPlatform30days/Day5/Step1/4.png)
5. Sign in with your credentials
![Credentials](/PowerPlatform/assets/PowerPlatform30days/Day5/Step1/5.png)
6. Enter your site URL or select from recent sites 
![Url SPO](/PowerPlatform/assets/PowerPlatform30days/Day5/Step1/6.png)
7. Select a list (e.g., `Requests`, `Employees`) and click in connect
![Select List](/PowerPlatform/assets/PowerPlatform30days/Day5/Step1/7.png)
8. The list is now connected to your app and visible in the data pane
![Select List](/PowerPlatform/assets/PowerPlatform30days/Day5/Step1/8.png)

---

### ✅ Step 3: Add an Excel Connector (Stored in OneDrive)

1. From the **Data** panel, click **+ Add data**
2. Search for **Excel Online (Business)** or **OneDrive for Business**
![Data and Add Data](/PowerPlatform/assets/PowerPlatform30days/Day5/NextSteps/Step3_1_2.png)
3. Sign in to your OneDrive account
![Sign in OneDrive](/PowerPlatform/assets/PowerPlatform30days/Day5/NextSteps/Step3_3.png)
4. Choose a Location in OneDrive for Business
![Choose Location](/PowerPlatform/assets/PowerPlatform30days/Day5/NextSteps/Step3_4.png)
5. Select OneDrive
![Select OneDrive](/PowerPlatform/assets/PowerPlatform30days/Day5/NextSteps/Step3_5.png)
6. Navigate to your Excel file (ensure it has **formatted tables**)
![Select the file](/PowerPlatform/assets/PowerPlatform30days/Day5/NextSteps/Step3_6.png)
7. Select the table(s) you want to use
![Select the table](/PowerPlatform/assets/PowerPlatform30days/Day5/NextSteps/Step3_7.png)
8. Insert auto generated id into Excel Table and connect 
![Add ID row](/PowerPlatform/assets/PowerPlatform30days/Day5/NextSteps/Step3_8.png)
9. Now you can use it with galleries, forms, and dropdowns

---

### ✅ Step 4: Connect to Dataverse Tables

1. From **make.powerapps.com**, go to **Tables** under Dataverse
2. Use a built-in table (e.g., `Account`) or create your own
3. In a Canvas app, open **Data** and add **Dataverse** or tables available in recent tables.
4. Choose the tables you want to use
![Add ID row](/PowerPlatform/assets/PowerPlatform30days/Day5/NextSteps/Step4_1.png)
5. Dataverse allows you to model complex relationships and secure your data
![Add ID row](/PowerPlatform/assets/PowerPlatform30days/Day5/NextSteps/Step4_2.png)

---

### ✅ Step 5: Use Connected Data in Your App

- Use **Gallery.Items = [YourDataSource]** to show data
![Use data source added](/PowerPlatform/assets/PowerPlatform30days/Day5/NextSteps/Step5_1.png)
- Use **Form.DataSource = [YourDataSource]** to edit records
- Use functions like **Patch**, **Collect**, **LookUp**, and **Filter** to interact with data
![Show data in different galleries](/PowerPlatform/assets/PowerPlatform30days/Day5/NextSteps/Step5_2.png)
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
