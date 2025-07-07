
# Day 16 – Variables, Conditions, and Loops in Power Automate

---

## 📝 Overview

In Power Automate, you can use **variables** to store and update values, **conditions** to add logic, and **loops** to perform repeated actions. These tools allow you to build powerful workflows that adapt to your data and business rules.

Today you'll learn how to initialize and modify variables, write conditional logic, and use `Apply to each` and `Do until` loops.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Initialize a Variable

1. In a new or existing flow, click **+ New step**
2. Search for **Initialize variable**
3. Set:
   - **Name**: `counter`
   - **Type**: Integer or String
   - **Value**: `0` (for numbers) or leave blank
4. This variable can now be updated later in the flow

---

### ✅ Step 2: Set or Increment a Variable

1. Add another step: **Increment variable** or **Set variable**
2. Choose the variable you initialized (e.g., `counter`)
3. Set value or increment amount:
   ```text
   Value = 1  (for increment)
   Value = "Completed" (for string set)
   ```

---

### ✅ Step 3: Add a Condition

1. Click **+ New step > Control > Condition**
2. Set a logic expression, such as:
   ```text
   counter is greater than 3
   ```
3. Inside **If yes** and **If no**, add the actions to perform depending on the result
4. Use **dynamic content** or expressions like `@equals(...)`, `@empty(...)`, etc.

---

### ✅ Step 4: Use an "Apply to each" Loop

1. Click **+ New step > Control > Apply to each**
2. Choose an array or collection (e.g., value from a SharePoint list)
3. Inside the loop, add the action(s) to perform for each item

---

### ✅ Step 5: Use a "Do Until" Loop

1. Click **+ New step > Control > Do until**
2. Set the **exit condition** (e.g., `counter` is greater than `5`)
3. Inside the loop:
   - Perform your actions
   - Increment the counter
4. Be sure to add a **timeout or limit** to avoid infinite loops

---

## 🔎 What You Should Try Today

- Initialize a variable and update it with values
- Add a condition to branch your flow logic
- Use a loop to perform actions on multiple items
- Combine variables, conditions, and loops into one flow

---

## 🔁 Navigation

⬅️ [**Go to Day 15: Power Automate – Creating automated, instant, and scheduled flows**](/PowerPlatform/Power%20Platform%2030%20days/Day15.md)  
➡️ [**Go to Day 17: Advanced use of expressions and error handling**](/PowerPlatform/Power%20Platform%2030%20days/Day17.md)
