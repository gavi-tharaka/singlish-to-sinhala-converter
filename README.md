🇱🇰 Singlish to Sinhala Unicode ConverterA lightweight, plug-and-play Vanilla JavaScript utility that seamlessly converts Singlish phonetics into Sinhala Unicode in real-time. It automatically attaches to any text input or textarea on your website, requiring absolutely no extra configuration.✨ FeaturesZero Dependencies: Pure Vanilla JavaScript. No jQuery, React, or Vue required (but fully compatible with them).Plug & Play: Just link the script, and it automatically works on all existing and future <input> and <textarea> fields.Smart Toggle: Easily switch between Sinhala and English typing modes using the Ctrl + Space keyboard shortcut.Framework Friendly: Emits standard native input events so state managers in React/Vue/Angular can catch the typing changes seamlessly.Lightweight: Highly optimized and fast execution without lagging the browser.🚀 How to Use (Installation)You can use this converter on your website in two ways: Online (CDN) or Local Download.Method 1: The Easiest Way (Online CDN)You don't need to download any files. Just copy and paste the following <script> tag into your HTML file, right before the closing </body> tag. It will load the script directly from GitHub via jsDelivr.<!-- Add this before closing </body> tag -->
<script src="https://cdn.jsdelivr.net/gh/gavi-tharaka/singlish-to-sinhala-converter@main/singlish.js"></script>
Method 2: Local HostingIf you prefer to host the script yourself:Download the singlish.js file from this repository.Place it in your project folder.Link it in your HTML:<script src="path/to/your/folder/singlish.js"></script>
💻 Usage & DemoOnce the script is added to your page, simply click on any input field and start typing in Singlish.Type in Singlish: e.g., typing kohomada will automatically output කොහොමද.Change Language Mode: Press Ctrl + Space to toggle between Sinhala and English typing modes at any time.HTML Example:<!DOCTYPE html>
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
    <script src="https://cdn.jsdelivr.net/gh/gavi-tharaka/singlish-to-sinhala-converter@main/singlish.js"></script>
</body>
</html>
🔔 Advanced: Listening to Mode Changes (For Developers)If you want to update your UI (like showing a badge "Sinhala Mode" or "English Mode") when the user presses Ctrl + Space, you can listen to the custom singlishModeChange event globally:document.addEventListener('singlishModeChange', function(event) {
    const isSinhala = event.detail.isSinhala; // returns true or false
    
    if (isSinhala) {
        console.log("Typing Mode: Sinhala");
        // Update your UI to show Sinhala mode
    } else {
        console.log("Typing Mode: English");
        // Update your UI to show English mode
    }
});
📝 Phonetic Cheat Sheet (Basic)Here are some standard combinations used in this converter:a = අ | aa / A = ආ / ඇi = ඉ | ii = ඊu = උ | uu = ඌk = ක් | ka = කg = ග් | ga = ගc / ch = ච් | cha = චt = ට් | th = ත්d = ඩ් | dh = ද්📄 LicenseThis project is open-source and available under the MIT License. Feel free to use it, modify it, and contribute!Developed by Tharaka.
