# 💻 DevbyJr | Custom Linktree Website

A sleek, minimal, and personal **Linktree-style website** for showcasing all of DevbyJr’s social and coding platforms in one place.  
Built from scratch using pure **HTML, CSS, and JavaScript** — no frameworks, just clean code.

---

## 🚀 Features

- 🧩 **Custom logo, name, and bio**
- 🎨 **Modern glassmorphism design**
- 📱 **Fully responsive (mobile-first)**
- ⚡ **Smooth fade-in and button animations**
- 🔗 **Clean button links for GitHub, YouTube, TikTok, and Instagram**
- ☁️ **Easily deployable with GitHub Pages**

---

## 🧱 Project Structure

```
linktree/
│
├── index.html        # Main page
├── comingsoon.html   # Coming soon page
├── projects.html     # Projects page
├── style.css         # Styles and animations
├── script.js         # Page animations and effects
├── images/           # Logo and images (logo filename: devbyjr-logo.png)
└── README.md         # This documentation
```

---

## 👤 About

**Name:** DevbyJr  
**Bio:** Self-taught dev in the making 💻  
**Email:** [devbyjr@hotmail.com](mailto:devbyjr@hotmail.com)

---

## 🔗 Links

These are the default platform buttons on the site.  
You can edit them directly in `index.html` inside the `<div class="links">`.

```html
<a href="https://github.com/DevbyJr" target="_blank">GitHub</a>
<a href="https://youtube.com/@DevbyJr" target="_blank">YouTube</a>
<a href="https://www.tiktok.com/@DevbyJr" target="_blank">TikTok</a>
<a href="https://www.instagram.com/DevbyJr" target="_blank">Instagram</a>
```

---

## 💅 Styling & Design

All styles are handled in `style.css` and can be fully customized:

- Background gradient
- Font families
- Link colors and hover effects
- Card shadows and border radius

### Example background (editable):

```css
body {
  background: linear-gradient(135deg, #1f1c2c, #928dab);
}
```

---

## 🪄 Animations (CSS + JS)

Your site includes smooth fade-in effects and clickable button animations using **CSS transitions** and **JavaScript events**.

### 🎨 Add this to `style.css`:

```css
.container {
  opacity: 0;
  transform: translateY(30px);
  transition: opacity 1s ease, transform 1s ease;
}

.container.fade-in {
  opacity: 1;
  transform: translateY(0);
}
```

### ⚙️ `script.js`

```js
// --- Fade-in Animation on Page Load ---
document.addEventListener("DOMContentLoaded", () => {
  const container = document.querySelector(".container");
  container.classList.add("fade-in");
});

// --- Smooth Button Click Animation ---
const links = document.querySelectorAll(".links a");
links.forEach((link) => {
  link.addEventListener("mousedown", () => {
    link.style.transform = "scale(0.96)";
  });
  link.addEventListener("mouseup", () => {
    link.style.transform = "scale(1)";
  });
});
```

### 💡 What It Does

- Fades in the entire page smoothly when it loads
- Adds a **press-down animation** when buttons are clicked
- Keeps the site lightweight and minimal with no analytics or dark mode

---

## 🧰 Tech Stack

- **HTML5**
- **CSS3**
- **JavaScript (ES6)**
- **GitHub Pages** for hosting

---

## 💡 Future Enhancements

- Add gradient theme selector
- Add link click counter
- Include sound or hover tones for buttons

---

## 🏁 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👨‍💻 Author

**DevbyJr**  
💼 Self-taught Developer in the Making 💻  
🐙 [GitHub](https://github.com/DevbyJr)  
▶️ [YouTube](https://youtube.com/@DevbyJr)  
🎵 [TikTok](https://www.tiktok.com/@DevbyJr)  
📸 [Instagram](https://www.instagram.com/DevbyJr)
🌐 [Discord](https://discord.gg/TTqrJxfxBe)
📧 [devbyjr@hotmail.com](mailto:devbyjr@hotmail.com)

---

⭐ **Star this repo** if you like the project or use it as a template for your own Linktree!
