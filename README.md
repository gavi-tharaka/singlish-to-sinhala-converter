# Singlish to Sinhala Unicode Converter

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow?logo=javascript)](#)
[![Live Demo](https://img.shields.io/badge/Live_Demo-View_Here-brightgreen?logo=googlechrome)](https://gavi-tharaka.github.io/singlish-to-sinhala-converter/)

> **🔗 [Click Here to Try the Live Demo](https://gavi-tharaka.github.io/singlish-to-sinhala-converter/)**

A lightweight, plug-and-play Vanilla JavaScript utility that seamlessly converts Singlish phonetics into Sinhala Unicode in real-time. It automatically attaches to any text input or textarea on your website, requiring absolutely no extra configuration.

## ✨ Features

- **Zero Dependencies:** Pure Vanilla JavaScript. No jQuery, React, or Vue required (but fully compatible with them).
- **Plug & Play:** Just link the script, and it automatically works on all existing and future `<input>` and `<textarea>` fields.
- **Smart Toggle:** Easily switch between Sinhala and English typing modes using the `Ctrl + Space` keyboard shortcut.
- **Framework Friendly:** Emits standard native `input` events so state managers in React/Vue/Angular can catch the typing changes seamlessly.
- **Lightweight:** Highly optimized and fast execution without lagging the browser.

---

## 🚀 How to Use (Installation)

You can use this converter on your website in two ways: **Online (CDN)** or **Local Download**.

### Method 1: The Easiest Way (Online CDN)
You don't need to download any files. Just copy and paste the following `<script>` tag into your HTML file, right before the closing `</body>` tag. It will load the script directly from GitHub via jsDelivr.

```html
<!-- Add this before closing </body> tag -->
<script src="https://cdn.jsdelivr.net/gh/gavi-tharaka/singlish-to-sinhala-converter@main/singlish.js"></script>
```

### Method 2: Local Hosting
If you prefer to host the script yourself:
1. Download the `singlish.js` file from this repository.
2. Place it in your project folder.
3. Link it in your HTML:

```html
<!-- Add this before closing </body> tag -->
<script src="path/to/your/folder/singlish.js"></script>
```

## 💻 Usage & Demo
- Once the script is added to your page, simply click on any input field and start typing in Singlish.
- Type in Singlish: e.g., typing kohomada will automatically output කොහොමද.
- Change Language Mode: Press Ctrl + Space to toggle between Sinhala and English typing modes at any time.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Singlish Converter Test</title>
</head>
<body>
    
    <h2>Singlish Typing Test</h2>
    <p>Press <b>Ctrl + Space</b> to switch between English and Sinhala.</p>

    <!-- It works automatically on these inputs! -->
    <input type="text" placeholder="Type here in Singlish..."><br><br>
    <textarea rows="4" cols="50" placeholder="Type a long paragraph..."></textarea>

    <!-- Link the CDN -->
    <script src="[https://cdn.jsdelivr.net/gh/gavi-tharaka/singlish-to-sinhala-converter@main/singlish.js](https://cdn.jsdelivr.net/gh/gavi-tharaka/singlish-to-sinhala-converter@main/singlish.js)"></script>
</body>
</html>
```

## 🔔 Advanced: Listening to Mode Changes (For Developers)
If you want to update your UI (like showing a badge "Sinhala Mode" or "English Mode") when the user presses `Ctrl + Space`, you can listen to the custom `singlishModeChange` event globally:
```js
document.addEventListener('singlishModeChange', function(event) {
    const isSinhala = event.detail.isSinhala; // returns true or false
    
    if (isSinhala) {
        console.log("Typing Mode: Sinhala");
        // Update your UI to show Sinhala mode
    } else {
        console.log("Typing Mode: English");
        // Update your UI to show English mode
    }
});
```

## 📝 Phonetic Cheat Sheet (Basic)
Here are some standard combinations used in this converter:

- a = අ | aa / A = ආ / ඇ
- i = ඉ | ii = ඊ
- u = උ | uu = ඌ
- k = ක් | ka = ක
- g = ග් | ga = ග
- c / ch = ච් | cha = ච
- t = ට් | th = ත්
- d = ඩ් | dh = ද්


## 📄 License
This project is open-source and available under the MIT License. Feel free to use it, modify it, and contribute!
Developed by [Gavindu Tharaka](https://github.com/gavi-tharaka).
