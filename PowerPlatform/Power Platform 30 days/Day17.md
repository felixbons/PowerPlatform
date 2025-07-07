
# Day 17 – Advanced Use of Expressions and Error Handling

---

## 📝 Overview

Power Automate supports powerful expressions using the **Workflow Definition Language**. These expressions allow you to manipulate strings, numbers, dates, and arrays dynamically. Pairing them with **error handling** features ensures your flows are resilient and informative when something goes wrong.

In this session, you'll learn how to use common advanced expressions, handle exceptions using **Configure run after**, and gracefully manage errors using scopes and parallel branches.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Use Expressions to Format Data

1. In any input field, click **Expression** (next to Dynamic content)
2. Example: Format today’s date
   ```text
   formatDateTime(utcNow(), 'yyyy-MM-dd')
   ```
3. Other common expressions:
   - `toLower(triggerOutputs()?['headers']['from'])`
   - `addDays(utcNow(), 3)`
   - `length(body('Get_items')?['value'])`

---

### ✅ Step 2: Nest Expressions

- Example: Return a fallback value if the input is blank
  ```text
  if(empty(triggerBody()?['Name']), 'Anonymous', triggerBody()?['Name'])
  ```

- Use `coalesce()` to return the first non-empty value:
  ```text
  coalesce(triggerBody()?['Email'], 'default@company.com')
  ```

---

### ✅ Step 3: Add a Scope for Grouping Actions

1. Add a **Scope** from **Control > Scope**
2. Place multiple actions inside (e.g., Get items + Send email)
3. Use scopes to logically group success or failure actions

---

### ✅ Step 4: Handle Errors with "Configure Run After"

1. Add an action after a Scope or step
2. Click the **three dots (⋮)** > **Configure run after**
3. Choose when this action should run:
   - After failure
   - After success
   - After skipped
4. Add a **Send email** or **Compose** step to notify on failure

---

### ✅ Step 5: Use Try-Catch-Like Error Handling

1. Create **two scopes**: `Try`, `Catch`
2. In `Try`, place your main flow logic
3. In `Catch`, place notification logic or fallback steps
4. Use **Configure run after** on `Catch` to only run if `Try` fails

---

## 🔎 What You Should Try Today

- Use `formatDateTime()` and `addDays()` to manipulate dates
- Use `if()` or `coalesce()` to avoid blank/null errors
- Create a Try-Catch structure using scopes
- Add a failure notification using `Configure run after`

---

## 🔁 Navigation

⬅️ [**Go to Day 16: Variables, conditions, and loops in Power Automate**](/PowerPlatform/Power%20Platform%2030%20days/Day16.md)  
➡️ [**Go to Day 18: Introduction to Dataverse – structure, tables, and relationships**](/PowerPlatform/Power%20Platform%2030%20days/Day18.md)
