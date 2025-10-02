
# Day 13 – Reusable Components and Master Screens

---

## 📝 Overview

Reusable components and master screens help maintain consistency, reduce development time, and simplify maintenance. With **Component Libraries** and **template screens**, you can create standardized headers, footers, menus, and dialogs that can be reused across multiple apps or screens.

Today, you'll learn how to create custom components, build master screen layouts, and import them into other apps to scale your development process.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Create a New Component

1. In Power Apps Studio, go to **Tree View > Components**.
2. Click **+ New component**.
3. Rename it `cmp_Header`.
4. Add:
   - A **Label** for the app title
   - An **Icon** (e.g., Home or Back button)
5. Set properties like `HeaderTitle` or `OnIconSelect` as **custom properties**:
   - Click **+ New custom property**
   - Name: `HeaderTitle` (Input, Text)
   - Name: `OnIconSelect` (Input, Event, Return Type = boolean)
   ![Firsts Steps](/PowerPlatform/assets/PowerPlatform30days/Day13/12-08-2025_22-06-00.png)
6. Bind label text and icon’s `OnSelect` to these properties.
   ![Last Step](/PowerPlatform/assets/PowerPlatform30days/Day13/12-08-2025_22-09-51.png)

---

### ✅ Step 2: Insert Component into Screens

1. Go to any screen in your app.
2. Click **Insert > Custom > cmp_Header**.
3. Set:
   ```powerfx
   HeaderTitle = "Dashboard"
   OnIconSelect = Navigate(HomeScreen)
   ```

---

### ✅ Step 3: Build a Master Screen Template

1. Create a screen named `scr_Template`.
2. Add shared layout elements:
   - Header (e.g., `cmp_Header`)
   - Navigation bar or footer
   - Background color or logo
3. Duplicate this screen to create new screens with consistent structure.

---

### ✅ Step 4: Use a Component Library (For Multi-App Use)

1. Go to **More > App enhancements > Component libraries > + New component library**
2. Create reusable components (header, footer, confirmation dialog, etc.)
3. In your app, go to **Insert > Get more components**
4. Import components from your library

---

### ✅ Step 5: Update Once, Use Everywhere

- When you update a component in the library:
  - All apps using that library will prompt you to apply updates
- This saves time and ensures UI/UX consistency across your organization

---

## 🔎 What You Should Try Today

- Create a custom header component with title and icon
- Add it to 2–3 screens and configure properties
- Build a template screen and duplicate it for consistency
- Explore creating your own component library for reuse across apps

---

## 🔁 Navigation

⬅️ [**Go to Day 12: Professional UX/UI design for Power Apps (visual tips)**](/PowerPlatform/Power%20Platform%2030%20days/Day12.md)  
➡️ [**Go to Day 14: Publishing, sharing, and permissions in a Canvas app**](/PowerPlatform/Power%20Platform%2030%20days/Day14.md)
