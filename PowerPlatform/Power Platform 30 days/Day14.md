
# Day 14 – Publishing, Sharing, and Permissions in a Canvas App

---

## 📝 Overview

Once your Power App is ready, it's time to **publish**, **share**, and manage **permissions** so others can use it. Power Apps provides flexible options for app visibility and control, including role-based permissions, versioning, and secure data access.

In this session, you’ll learn how to publish updates, share your app with individual users or groups, and configure permissions to ensure your app is used safely and efficiently.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Save and Publish Your Canvas App

1. Click **Save** button to ensure all changes are saved.
   ![Save](/PowerPlatform/assets/PowerPlatform30days/Day14/Step1_1.png)
2. Go to **Publish**.
3. Click **Publish this version** to make changes live for users.
   ![Publish](/PowerPlatform/assets/PowerPlatform30days/Day14/Step1_2.png)

---

### ✅ Step 2: Share the App with Users

1. Go to **Share**.
![Share](/PowerPlatform/assets/PowerPlatform30days/Day14/Step2_1.png)
2. Enter the email addresses of users or security groups.
3. Set their role:
   - **User**: can run the app
   - **Co-owner**: can edit and manage the app
4. Click **Share** to grant access.
![Complete Share](/PowerPlatform/assets/PowerPlatform30days/Day14/Step2_2.png)

> ✅ Tip: Use security groups in Entra ID to simplify large-scale sharing.

---

### ✅ Step 3: Manage App Permissions

1. From [https://make.powerapps.com](https://make.powerapps.com), go to **Apps**.
2. Click the **three dots (⋮)** on your app
3. Click in **Share**.
![three dots](/PowerPlatform/assets/PowerPlatform30days/Day14/Step3_1.png)
4. Type the name, email or security groups.
5. Set their role:
   - **User**: can run the app
   - **Co-owner**: can edit and manage the app
6. Review or modify permissions for each user or group.
7. Remove access by clicking the **Manage Access** before to Copy Link. 
![Add user](/PowerPlatform/assets/PowerPlatform30days/Day14/Step3_2.png)
8. Then in the drop down next to the user click in remove user and click in Share.
![Add user](/PowerPlatform/assets/PowerPlatform30days/Day14/Step3_3.png)

---

### ✅ Step 4: Monitor App Usage

1. Go to **Monitor > Overview** in the Power Platform admin center.
2. First time, turn on the tenant-wide analitycs, it will show the direct link to turn on.
2. Select your app to see:
   - User activity
   - Error rates
   - Sessions over time
3. Use insights to improve app performance and usability.

---

### ✅ Step 5: Secure Data Sources

1. Go to **Data > Connections**.
2. Ensure only authorized users have access to the app’s data connectors (SharePoint, Dataverse, etc.).
3. For SharePoint, set item-level permissions if needed.
4. For Dataverse, configure table-level and column-level security.

---

## 🔎 What You Should Try Today

- Save and publish your app with a meaningful version name
- Share it with at least one other user for testing
- Review app usage in Analytics
- Restrict or update data permissions for a key data source

---

## 🔁 Navigation

⬅️ [**Go to Day 13: Reusable components and master screens**](/PowerPlatform/Power%20Platform%2030%20days/Day13.md)  
➡️ [**Go to Day 15: Power Automate – Creating automated, instant, and scheduled flows**](/PowerPlatform/Power%20Platform%2030%20days/Day15.md)
