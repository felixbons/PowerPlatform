
# Day 8 – Controls: Forms, Galleries, Buttons, Dropdowns

---

## 📝 Overview

Controls are the interactive building blocks of Power Apps. They let users view data, input information, perform actions, and navigate between screens. The most commonly used controls include:

- **Galleries**: Display a list of records visually.
- **Forms**: Show or edit a single record.
- **Buttons**: Trigger logic such as saving data or navigating screens.
- **Dropdowns**: Allow users to choose from a list of values.

In this session, you'll learn how to add and configure these controls, connect them to your data sources, and create basic app functionality.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Add a Gallery to Display Data

1. Go to [https://make.powerapps.com](https://make.powerapps.com) and open or create a Canvas app.
2. In the left menu, click **Insert** > **Gallery** > **Vertical**.
3. From the right panel, choose your **Data Source** (e.g., SharePoint, Excel, Dataverse).
4. Set the **Items** property of the gallery:
   ```powerfx
   Items = Employees
   ```
5. Customize the gallery layout using the pane or by selecting controls inside the gallery (e.g., labels, images).

![Add Gallery](/PowerPlatform/assets/PowerPlatform30days/Day8/Step1_2.png)


---

### ✅ Step 2: Add an Edit Form for Record Updates

1. Go to **Insert** > **Forms** > **Edit Form**.
2. Place it below or beside the gallery.
3. Set the form’s **DataSource**:
   ```powerfx
   DataSource = Employees
   ```
4. Set the form’s **Item** property:
   ```powerfx
   Item = gal_Employees.Selected
   ```
5. In the right pane, click **Edit fields** to choose which columns to show.
6. Optionally, switch to a **Display Form** to make it read-only.

![Form](/PowerPlatform/assets/PowerPlatform30days/Day8/Step2.png)

---

### ✅ Step 3: Add a Button to Submit the Form

1. Go to **Insert** > **Button**.
2. Set the button’s **Text** property to `"Save"` or `"Submit"`.
3. Set its **OnSelect** action:
   ```powerfx
   OnSelect = SubmitForm(Form_Employee)
   ```
4. Optional: Add a confirmation label and set it to display a success message:
   ```powerfx
   Label.Text = "Record saved successfully!" or
   Notify("Record saved successfully!",NotificationType.Success)
   ```

5. Go to **Insert** > **Button**.
6. Set the button’s **Text** property to `"New"`.
7. Set its **OnSelect** action:
   ```powerfx
   OnSelect = NewForm(Form_Employee)
   ```
8. Adjust the button next to Submit button. 

![Form](/PowerPlatform/assets/PowerPlatform30days/Day8/Step3.png)
---

### ✅ Step 4: Add a Dropdown Control

1. Go to **Insert** > **Input** > **Dropdown**.
2. Set the **Items** property for static values:
   ```powerfx
   ["HR", "Finance", "IT"]
   ```
   Or pull values from a data column dynamically:
   ```powerfx
   Distinct(Employees, Department)
   ```
3. Use the selected value elsewhere in your app:
   ```powerfx
   Label.Text = dd_Department.Selected.Value
   ```

---

### ✅ Step 5: Test the Controls Together

- Use the **Play** button (▶️) to preview the app.
- Select a record from the gallery — confirm it appears in the form.
- Change a field and click the **Save** button.
- Try filtering the gallery using the selected value from the dropdown.

---

## 🔎 What You Should Try Today

- Connect a gallery to your data and display key fields.
- Use an edit form to show the selected item.
- Add a button to submit form data.
- Add a dropdown and use it to filter or categorize records.

---

## 🔁 Navigation

⬅️ [**Go to Day 7: Best practices for working with the Power Platform interface**](/PowerPlatform/Power%20Platform%2030%20days/Day07.md)  
➡️ [**Go to Day 9: Variables and context (Set, UpdateContext, Navigate)**](/PowerPlatform/Power%20Platform%2030%20days/Day09.md)
