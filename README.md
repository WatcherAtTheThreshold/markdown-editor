# Markdown Editor

A minimal, focused Markdown editor built for clarity and speed. This tool provides a bridge between a quiet, "Zen-like" writing environment and the power of full Markdown/WYSIWYG editing.

## ✨ Key Features

* **Dual-Mode Editing:** Seamlessly switch between a **WYSIWYG** (What You See Is What You Get) interface and a raw **Markdown** editor.
* **Auto-Generated Navigation:** Your document's `##` headings are automatically turned into a clickable table of contents in the sidebar.
* **Local Persistence:** Never lose a word. The editor automatically saves drafts to your browser's `localStorage` as you type.
* **Sidebar Navigation:** Sidebar "jump-to-section" feature to navigate long documents instantly.
* **Print-Ready Styles:** A custom print engine that formats your Markdown into a clean, professional PDF-ready document.
* **File Interoperability:** Easily **Import** existing `.md` files or **Export** your work as a `README.md`.
* **Flexible Exporting:** Includes a dedicated filename field that defaults to README.md for repository convenience, allowing you to name your exports (e.g., TODO.md, CHANGELOG.md) before downloading.

## 🚀 Getting Started

1. **Open the Editor:** Simply open `index.html` in any modern web browser, at [https://watcheratthethreshold.github.io/markdown-editor/](https://watcheratthethreshold.github.io/markdown-editor/).
2. **Write:** Start typing in the main pane. Use the toolbar for formatting or type raw Markdown.
3. **Navigate:** Click on section titles in the left sidebar to quickly jump to different parts of your document.
4. **Save & Export:** \* **Autosave:** The editor automatically saves your work as a draft in your browser's local storage.
    * **Custom Naming:** Type a custom filename (e.g., `TODO.md`) into the field next to the Export button.
    * **Download:** Press `Ctrl + S` (or `Cmd + S`) or click **Export** to download your file.


## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
| -------- | ------ |
| `Ctrl` + `S` | Export as `README.md` |
| `Enter` | New line / New list item |
| `Tab` | Indent list / Code block |

## 🛠️ Technical Overview

The project is modularized for easy maintenance:

* **`nav.js`**: Handles the logic for parsing Markdown headings and managing editor scroll/focus.
* **`storage.js`**: Manages the `localStorage` API for draft persistence.
* **`io.js`**: Handles file reading (Import) and Blob generation (Export).
* **`app.js`**: The main orchestrator that initializes the Toast UI Editor and wires up the UI events.
* **`style.css`**: A custom "quiet UI" theme featuring a backdrop-blur topbar and a responsive grid layout.

## 🎨 Customizing the Look

The editor uses CSS variables for easy theming. You can modify the colors in `style.css` under the `:root` selector:

```css
:root {
  --bg: #fbfaf8;    /* Background color */
  --ink: #141414;   /* Text color */
  --panel: #ffffff; /* Sidebar & Editor background */
}
```
***

*Last updated: December 2025*

***
