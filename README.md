# Portfolio Website - Tailwind Dark/Light Mode Enhancement

## Overview
This project is a personal portfolio website. Recently, the site was enhanced to support both dark and light modes using Tailwind CSS, making it more modern and user-friendly. This README explains all the changes made, step by step, in beginner-friendly language.

---

## What Was Changed?

### 1. Added Tailwind CSS
- **What is Tailwind?**
  - Tailwind CSS is a utility-first CSS framework that lets you style your website quickly using special class names in your HTML.
- **How was it added?**
  - A link to the Tailwind CDN (Content Delivery Network) was added in the `<head>` section of each HTML file. This lets you use Tailwind classes without installing anything.
  - Example:
    ```html
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@3.4.1/dist/tailwind.min.css" rel="stylesheet">
    ```

### 2. Implemented Dark/Light Mode Toggle
- **What is dark/light mode?**
  - Dark mode changes the website background and text to darker colors, which is easier on the eyes in low light. Light mode uses lighter backgrounds and darker text.
- **How does the toggle work?**
  - A button (with a sun/moon icon) was added to the navigation bar on every page.
  - When you click the button, it switches the website between dark and light mode.
  - Your choice is saved, so if you come back later, the site remembers your preference.

### 3. How the Code Works
- **Tailwind Classes:**
  - The `<body>` tag now has these classes:
    - `bg-white text-gray-900` for light mode (white background, dark text)
    - `dark:bg-gray-900 dark:text-white` for dark mode (dark background, white text)
    - `transition-colors duration-300` for smooth color changes
- **Toggle Button:**
  - The button uses Tailwind classes for styling and shows a sun or moon icon depending on the mode.
- **JavaScript:**
  - A script was added at the bottom of each HTML file. It:
    1. Checks if you have a saved theme (dark or light) in your browser.
    2. If not, it checks your system preference (if your computer prefers dark mode).
    3. When you click the toggle button, it adds or removes the `dark` class on the `<html>` element, switching the mode.
    4. It saves your choice for next time.

### 4. Consistent Navigation
- The navigation bar on every page was updated to use Tailwind classes for a modern look and to include the dark/light toggle button.

---

## How to Use
1. **Open any page** (e.g., `index.html`, `about.html`, etc.) in your browser.
2. **Find the toggle button** (sun/moon icon) in the top navigation bar.
3. **Click the button** to switch between dark and light mode.
4. **Your choice is remembered** even if you close and reopen the browser.

---

## Why These Changes?
- **Modern look:** Tailwind makes the site look more professional and clean.
- **Accessibility:** Dark mode is easier on the eyes for many users.
- **User experience:** Remembering the user's theme preference makes the site feel more personal.

---

## Next Steps
- You can further customize colors, add animations, or use more Tailwind features to improve your site.
- Explore Tailwind's documentation for more ideas: https://tailwindcss.com/docs

---

## Questions?
If you have any questions or want to learn more, feel free to ask!
