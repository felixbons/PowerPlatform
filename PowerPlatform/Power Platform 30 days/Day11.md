
# Day 11 – CRUD Operations with SharePoint and Excel (Create, Read, Update, Delete)

---

## 📝 Overview

CRUD stands for **Create, Read, Update, Delete** — the core operations used when working with data. In Power Apps, you can perform these actions using SharePoint lists or Excel tables as your data source.

In this session, you'll learn how to connect your app to SharePoint and Excel, use galleries and forms to view and manage data, and use Power Fx functions like `Patch()`, `Remove()`, and `SubmitForm()` to perform CRUD operations.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Connect to a SharePoint List or Excel Table

1. Open [https://make.powerapps.com](https://make.powerapps.com)
2. Open or create a Canvas app
3. Go to **Data** > **+ Add data**
4. Search for and connect to:
   - A SharePoint list (e.g., `Employees`)
   - An Excel file stored in OneDrive (with a formatted table)

![Add Data](/PowerPlatform/assets/PowerPlatform30days/Day11/Step1.png)

---

### ✅ Step 2: Read Data (R)

1. Insert a **Gallery** (e.g., Vertical layout)
2. Set its **Items** property to your data source:
   ```powerfx
   Items = Employees
   ```
3. Customize labels inside the gallery to show data fields (e.g., Title, Department)

![Read data](/PowerPlatform/assets/PowerPlatform30days/Day11/Step2.png)

---

### ✅ Step 3: Create a Record (C)

**Option 1: Using a Form**
1. Insert an **Edit Form** and set:
   ```powerfx
   DataSource = Employees
   ```
2. Set **DefaultMode** to:
   ```powerfx
   FormMode.New
   ```
3. Use a **Submit** button with:
   ```powerfx
   SubmitForm(EditForm1)
   ```
![Create a Record](/PowerPlatform/assets/PowerPlatform30days/Day11/Step3_1.png)

**Option 2: Using `Patch()`**
1. Add text inputs: `txt_Name`, `txt_Department`
2. Use this formula in a button:
   ```powerfx
   Patch(Employees, Defaults(Employees), {
       Title: txt_Name.Text,
       Department: txt_Department.Text
   })
   ```
![use Patch](/PowerPlatform/assets/PowerPlatform30days/Day11/Step3_2.png)

---

### ✅ Step 4: Update a Record (U)

1. Add another **Edit Form**
2. Set **Item** property:
   ```powerfx
   Item = gal_Employees.Selected
   ```
3. Use a **Submit** button with:
   ```powerfx
   SubmitForm(EditForm1)
   ```
   This updates the selected record.
![Update a Record](/PowerPlatform/assets/PowerPlatform30days/Day11/Step4.png)

---

### ✅ Step 5: Delete a Record (D)

1. Add a **Trash icon** or button in the gallery
2. Set its **OnSelect**:
   ```powerfx
   Remove(Employees, <Gallery>.Selected)
   ```
![Delete a Record](/PowerPlatform/assets/PowerPlatform30days/Day11/Step5.png)

---

## 🔎 What You Should Try Today

- Connect to both a SharePoint list and Excel table
- Display data in a gallery
- Add a form or use `Patch()` to create new records
- Enable editing and deleting using gallery selections
- Explore differences between Excel and SharePoint limitations (e.g., delegation)

---

## 🔁 Navigation

⬅️ [**Go to Day 10: Validations, notifications, and common errors**](/PowerPlatform/Power%20Platform%2030%20days/Day10.md)  
➡️ [**Go to Day 12: Professional UX/UI design for Power Apps (visual tips)**](/PowerPlatform/Power%20Platform%2030%20days/Day12.md)
