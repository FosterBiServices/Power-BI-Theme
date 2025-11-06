
# Dynamic Power BI Theme

This repository provides a dynamic and customizable Power BI theme system using a template-based JSON file and an update script. It allows users to easily modify the primary color palette while preserving the integrity of the theme structure.

---

## 🎯 Purpose

To enable users to safely customize the primary colors of a Power BI theme without altering critical default settings or breaking the theme structure.

---

## 📁 Repository Contents

- `Theme Template.json` – A dynamic theme template with placeholder variables for easy customization.
- `Template Updates.ipynb` – A Jupyter Notebook script that processes the template and generates a finalized theme file.

---

## 🎨 Customization Instructions

1. Open `Theme Template.json` in a text editor.
2. Locate the first **8 colors** in the `"dataColors"` array.
3. Replace **only** these first 8 color values with your desired hex codes (e.g., `"#FF5733"`).
   - ✅ **Do**: Replace the first 8 colors.
   - ❌ **Do not**: Remove or add colors.
   - ❌ **Do not**: Modify any colors beyond the first 8.
4. **Do not change** the `themeColors` variables. These are essential for updating icon and default UI colors throughout the theme.

---

## ⚙️ Running the Update Script

1. Open `Template Updates.ipynb` in Jupyter Notebook or a compatible editor (e.g., VS Code with Jupyter extension).
2. Run all cells in the notebook.
3. The script will:
   - Replace placeholder variables like `themeColors` with the updated values.
   - Generate a finalized theme JSON file.
4. After the script completes, you may **rename the output file** as needed.

---

## ✅ Final Notes

- The theme file must contain **at least the original number of colors**.
- The `themeColors` variables are critical for consistent styling across Power BI visuals.
- Always validate the final theme in Power BI before sharing or deploying.


