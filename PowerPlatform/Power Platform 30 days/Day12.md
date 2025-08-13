
# Day 12 – Professional UX/UI Design for Power Apps (Visual Tips)

---

## 📝 Overview

User experience (UX) and user interface (UI) design are critical for app adoption and usability. A well-designed app is intuitive, accessible, and visually appealing — reducing user errors and improving satisfaction.

Today you'll learn visual design best practices for Power Apps, including layout consistency, spacing, colors, fonts, icons, and responsiveness.

---

## 🧭 Step-by-Step Guide

### ✅ Step 1: Use Consistent Spacing and Alignment

1. Use **containers** to group related controls.
2. Align labels, inputs, and buttons using the **Align** tools in the top ribbon.
3. Keep consistent padding (10–20px) between elements.
4. Avoid crowding — add breathing space around sections.

---

### ✅ Step 2: Apply a Color Palette

1. Define a small set of brand or theme colors, also you can use a function to call the theme:
   - Primary: `#0078D4` (blue)
   - Secondary: `#F3F2F1` (light gray)
   - Accent/Error: `#D13438` (red)

2. Apply color using the **Fill** and **BorderColor** properties:
   ```powerfx
   Fill = ColorValue("#F3F2F1")
   ```
3. Use contrast for accessibility — light backgrounds with dark text.
[Check for more information](https://accessibility.umich.edu/basics/concepts-principles/contrast)

4. Use a formula to centralize the information, allowing for quick and easy theme updates
   ```powerfx
   ----Formula-----
   varTheme = {
      Primary: RGBA(123, 134, 144, 1),
      Secondary: RGBA(134, 134, 144, 1)
   };

   ----How to implement-----
   varTheme.Primary
   ```
---

### ✅ Step 3: Use Standard Fonts and Font Sizes

1. Set headings to `Font.Size = 20–24`
2. Use `Font.Size = 14–16` for body text
3. Avoid mixing too many fonts — stick with **Segoe UI**, **Arial**, or **Roboto**

---

### ✅ Step 4: Add Icons and Visual Cues

1. Insert icons from **Insert > Icons** (e.g., Save, Trash, Home)
2. Use icons for:
   - Navigation
   - Submit/Delete buttons
   - Visual status indicators
3. Combine icons with labels for clarity:
   ```powerfx
   Icon + Label (side by side inside a container)
   ```
![Buttons Examples](/PowerPlatform/assets/PowerPlatform30days/Day12/12-08-2025_21-56-22.png)
---

### ✅ Step 5: Create Reusable Components

1. Create a **Component Library** via **Apps > Component Library**
2. Build:
   - Header bars
   - Footer navigation
   - Buttons with tooltips
3. Import components into any app for consistency

---

### ✅ Step 6: Optimize for Mobile vs Desktop

1. Choose **Phone** layout for mobile-first apps
2. Test responsiveness by resizing the editor window
3. Use containers and flexible width/height:
   ```powerfx
   Width = Parent.Width * 0.5
   ```

---

## 🔎 What You Should Try Today

- Create a header section with title and icon
- Apply a consistent color theme to your app
- Adjust font sizes and spacing for better readability
- Build and use at least one component
- Preview the app on desktop and mobile resolution

---

## 🔁 Navigation

⬅️ [**Go to Day 11: CRUD operations with SharePoint and Excel (Create, Read, Update, Delete)**](/PowerPlatform/Power%20Platform%2030%20days/Day11.md)  
➡️ [**Go to Day 13: Reusable components and master screens**](/PowerPlatform/Power%20Platform%2030%20days/Day13.md)
