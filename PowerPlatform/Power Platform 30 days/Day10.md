
# Day 10 – Validations, Notifications, and Common Errors

---

## 📝 Overview

Validating user input and providing real-time feedback is essential for creating reliable and user-friendly Power Apps. You can ensure data quality and improve the user experience by using functions like `IsBlank()`, `Len()`, and `Notify()`.

In this session, you’ll learn how to validate fields, display error or success messages, and handle common errors in Power Apps effectively.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Validate Required Fields

1. Insert a **Text input** control and name it `txt_Name`.
2. Insert a **Button** labeled `"Submit"`.
3. Set the Button’s **OnSelect** property:
   ```powerfx
   If(
       IsBlank(txt_Name.Text),
       Notify("Name is required", NotificationType.Error),
       Notify("Submission successful", NotificationType.Success)
   )
   ```
4. Try clicking the button with and without typing into the text input to test the logic.

![Step1](/PowerPlatform/assets/PowerPlatform30days/Day10/Step1.png)

---

### ✅ Step 2: Use Conditional Formatting for Visual Cues

1. Add a **Label** below the input.
2. Set its **Text** property:
   ```powerfx
   If(IsBlank(txt_Name.Text), "Please enter your name", "")
   ```
3. Set the **Color** property to red:
   ```powerfx
   If(IsBlank(txt_Name.Text), Color.Red, Color.Transparent)
   ```
![Step2](/PowerPlatform/assets/PowerPlatform30days/Day10/Step2.png)
---

### ✅ Step 3: Disable Submit Button Until Valid

1. Use the following in the **DisplayMode** property of the Submit button:
   ```powerfx
   If(IsBlank(txt_Name.Text), DisplayMode.Disabled, DisplayMode.Edit)
   ```
![Step3](/PowerPlatform/assets/PowerPlatform30days/Day10/Step3.png)
---

### ✅ Step 4: Handle Form Errors

1. Insert an **Edit Form** connected to a data source.
2. Add a **Submit button** and set the **OnSelect** property:
   ```powerfx
   SubmitForm(EditForm1)
   ```
3. Add a **Label** and set its **Text** property:
   ```powerfx
   EditForm1.Error
   ```
4. This will show backend errors if submission fails (e.g., required fields, connection issues).

![Step4](/PowerPlatform/assets/PowerPlatform30days/Day10/Step4.png)

---

### ✅ Step 5: Use Notify for Custom Messages

- Show a success message:
  ```powerfx
  Notify("Record saved!", NotificationType.Success)
  ```

- Show a warning:
  ```powerfx
  Notify("Please double-check your inputs", NotificationType.Warning)
  ```

- Show an error:
  ```powerfx
  Notify("An error occurred while submitting", NotificationType.Error)
  ```

---

## 🔎 What You Should Try Today

- Add validation to required fields using `IsBlank()`
- Display error messages dynamically using labels
- Use `Notify()` to provide success and error feedback
- Disable buttons when inputs are invalid
- Test a form with missing required fields to see backend errors

---

## 🔁 Navigation

⬅️ [**Go to Day 9: Variables and context (Set, UpdateContext, Navigate)**](/PowerPlatform/Power%20Platform%2030%20days/Day09.md)  
➡️ [**Go to Day 11: CRUD operations with SharePoint and Excel (Create, Read, Update, Delete)**](/PowerPlatform/Power%20Platform%2030%20days/Day11.md)
