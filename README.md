# Catalog Companion - PS 370

Catalog Companion is a simple, single-page web application designed to help families of PS 370 browse available items and submit orders easily. It replaces paper forms with a user-friendly digital interface that generates pre-formatted email orders.

## 🚀 Live Demo

[**Click here to view the live Catalog Companion**](https://justmark21.github.io/Catalog_Companion/)

## ✨ Features

* **Visual Catalog:** Browse 54+ items with images and descriptions.
* **Instant Search:** Quickly find items by name (e.g., "Rice", "Tuna") or ID number.
* **Simple Selection:** Click items to add them to a "shopping cart" style selection tray.
* **Order Form:** Collects necessary details:
  * Student & Parent Name
  * Household Size
  * Allergies
* **Smart Submission:**
  * **One-Click Email:** Automatically opens the user's default email app with a pre-written order.
  * **Webmail Support:** Dedicated buttons to open Gmail or Outlook in the browser.
  * **Clipboard Fallback:** "Copy Order Text" button for manual pasting if email apps fail.
* **Mobile Friendly:** Fully responsive design that works great on phones, tablets, and computers.

## 📂 Project Structure

This project is designed to be extremely simple. It runs entirely in the browser with no backend server required.

```text
/ (root folder)
├── index.html        # The main application code
├── images/           # Folder containing product images
│   ├── 1.jpg
│   ├── 2.jpg
│   ├── ...
│   └── 54.jpg
└── README.md         # This file

**Part 4: Setup & Deploy**
```markdown
## 🛠️ How to Set Up & Deploy

### 1. Upload Code

Upload the `index.html` file to your GitHub repository.

### 2. Add Images

The code is set to look for images in an `images/` folder.

1. Create a folder named `images` in your repository.
2. Upload your product photos into this folder.
3. **Important:** You must rename your image files to match the Item ID numbers found in the code (e.g., `1.jpg`, `2.jpg`, `3.jpg`, etc.).

### 3. Enable GitHub Pages

To make the website accessible to everyone:

1. Go to your repository **Settings**.
2. Click on **Pages** in the left sidebar.
3. Under **Branch**, select `main` (or `master`) and keep the folder as `/ (root)`.
4. Click **Save**.
5. Wait a minute, and GitHub will provide you with a live URL (e.g., `https://yourusername.github.io/repo-name/`).

## ⚙️ Customization

### Adding/Removing Items

To edit the catalog, open `index.html` and look for the `const catalogItems` array (around line 350).

**To add an item:**
Add a new line inside the list:
```javascript
{ id: 55, name: "New Item Name", category: "Snacks" },

Remember to add a corresponding 55.jpg to your images folder!

Changing the Email Address
If you need to change the recipient email address:

Search index.html for CatalogCompanionPS370@outlook.com.

Replace it with the new email address in both locations (the "Tip" text and the JavaScript logic).


**Part 6: Usage & License**
```markdown
## 📝 Usage Guide

1. **Select:** Users tap items to highlight them.
2. **Review:** A bar appears at the bottom showing the count of selected items.
3. **Submit:** Clicking "Review & Submit" opens the form.
4. **Send:** After filling in details, users choose their email provider (Default, Gmail, or Outlook) to send the order.

## 📄 License

This project is licensed under the MIT License.

