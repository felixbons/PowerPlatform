
# Day 9 – Variables and Context (`Set`, `UpdateContext`, `Navigate`)

---

## 📝 Overview

Variables allow your app to temporarily store values such as user input, selected items, or computed results. In Power Apps, there are **three key functions** used to manage variables and app behavior:

- `Set()` – defines a **global variable** usable across all screens.
- `UpdateContext()` – defines a **local/context variable** usable only in the current screen.
- `Navigate()` – moves the user between screens and can also pass variables to the destination.

Understanding these functions helps control your app's logic, flow, and data handling.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Create a Global Variable with `Set()`

1. Insert a **Button** into your screen.
2. Set the **OnSelect** property:
   ```powerfx
   Set(varUserName, "Felix")
   ```
3. Add a **Label** and set its **Text** property:
   ```powerfx
   varUserName
   ```
4. Preview the app, click the button, and observe the label show `"Felix"`.

---

### ✅ Step 2: Create a Local Variable with `UpdateContext()`

1. Insert another **Button**.
2. Set its **OnSelect** property:
   ```powerfx
   UpdateContext({ showPopup: true })
   ```
3. Add a **Label** and set its **Visible** property:
   ```powerfx
   showPopup
   ```
4. This label will only be visible when `showPopup` is true — the context variable exists only on this screen.

---

### ✅ Step 3: Navigate Between Screens Using `Navigate()`

1. Create two screens: `HomeScreen` and `DetailsScreen`.
2. Add a **Button** to `HomeScreen`.
3. Set the **OnSelect** property:
   ```powerfx
   Navigate(DetailsScreen, ScreenTransition.Fade, { userId: 12345 })
   ```
4. On `DetailsScreen`, insert a **Label** and set its **Text** property:
   ```powerfx
   userId
   ```
5. This shows how you can pass data between screens via the third parameter in `Navigate()`.

---

### ✅ Step 4: Clear or Reset Variables

- To reset a variable:
  ```powerfx
  Set(varUserName, Blank())
  ```
- To reset a context variable:
  ```powerfx
  UpdateContext({ showPopup: false })
  ```

---

## 🔎 What You Should Try Today

- Use `Set()` to store and display a name
- Use `UpdateContext()` to control the visibility of a control
- Pass data using `Navigate()` and display it on another screen
- Reset variables based on user interaction

---

## 🔁 Navigation

⬅️ [**Go to Day 8: Controls – Forms, galleries, buttons, dropdowns**](/PowerPlatform/Power%20Platform%2030%20days/Day08.md)  
➡️ [**Go to Day 10: Validations, notifications, and common errors**](/PowerPlatform/Power%20Platform%2030%20days/Day10.md)
