
# Day 21 – Dataverse Security: Roles, Permissions, and Column-Level Security

---

## 📝 Overview

Dataverse provides a powerful security model that protects data at the **table**, **record**, and **column** levels. Using **security roles**, **teams**, and **permissions**, you can control who can view, create, or modify specific data.

In this session, you'll learn how to manage security roles, apply permissions to tables and columns, and protect sensitive business data in your Power Platform environment.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Understand Security Layers

- **Environment security**: Who can create apps, flows, tables
- **Table security**: Who can read/write/delete data in a table
- **Row-level security**: Who can access specific records (via ownership)
- **Column-level security**: Restrict access to sensitive fields

---

### ✅ Step 2: Assign Security Roles

1. Go to [https://admin.powerplatform.microsoft.com](https://admin.powerplatform.microsoft.com)
2. Choose your environment > Click **Settings**
3. Go to **Users + permissions > Security roles**
4. Select an existing role (e.g., Common Data Service User) or click **New role**
5. Assign the role to users or security groups:
   - Go to **Users**
   - Select user > Click **Manage roles**

---

### ✅ Step 3: Set Table Permissions

1. In [https://make.powerapps.com](https://make.powerapps.com), go to **Tables**
2. Select a table > Click **Table permissions**
3. Configure create, read, write, delete permissions:
   - None
   - User
   - Business unit
   - Organization
4. Save and publish changes

---

### ✅ Step 4: Apply Column-Level Security

1. Open your table > Go to **Columns**
2. Select a column (e.g., `Salary`, `SSN`)
3. Click **Column security > Enable column security**
4. Create or assign **Field Security Profiles** in the admin center:
   - [Power Platform Admin Center > Security > Field security profiles](https://admin.powerplatform.microsoft.com)

---

### ✅ Step 5: Test Security as a User

1. Create a test user with limited permissions
2. Assign them only selected roles
3. Try accessing data in Power Apps or Model-driven app
4. Confirm field restrictions, access limits, or errors

---

## 🔎 What You Should Try Today

- Review existing security roles in your environment
- Apply table-level restrictions to a sensitive table
- Enable column security for a sensitive field
- Assign and test a user with limited permissions

---

## 🔁 Navigation

⬅️ [**Go to Day 20: Power Automate + Dataverse – build connected flows**](/PowerPlatform/Power%20Platform%2030%20days/Day20.md)  
➡️ [**Go to Day 22: Model-Driven Power Apps – structure and business logic**](/PowerPlatform/Power%20Platform%2030%20days/Day22.md)
