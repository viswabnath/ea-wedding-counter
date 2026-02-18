

# 💍 Anil & Eswari's Wedding Celebration — #EAParinayam

> A royal, fully static digital keepsake designed for Anil & Eswari's big day. Transitioned from a live countdown to a permanent digital memory.

---

## ✨ Features

* **👑 Royal Aesthetics** — High-end **Red & Gold** visual identity using the *Cinzel* (royal serif) and *Great Vibes* (script) font families.
* **📱 Smart Mobile Optimization** — The layout is anchored to the bottom of the screen on mobile devices, ensuring the couple's faces in the background photo remain perfectly visible.
* **⏳ Time-Aware UI** — Logic automatically switches the interface from "The Big Day Is Coming" to **"Happily Married!"** based on the wedding timestamp.
* **🌸 Interactive Petal Engine** — Lightweight JavaScript-driven animation that creates drifting red and pink petals across the screen.
* **🎨 Glassmorphism Design** — Features a frosted glass effect (`backdrop-filter: blur`) that ensures text readability over the background photo.

---

## 🛠 Technologies Used

| Layer | Technology |
| --- | --- |
| Structure | HTML5 |
| Styling | CSS3 (Flexbox, `clamp()`, Glassmorphism, Animations) |
| Fonts | Google Fonts — **Cinzel**, **Great Vibes**, **Montserrat** |
| Logic | Vanilla JavaScript |
| Hosting | GitHub Pages |

---

## 📁 Project Structure

```text
ea-wedding-counter/
├── index.html              # Main application file (HTML + CSS + JS)
├── background.jpg          # Couple background photo (Royal Theme)
├── README.md               # Project documentation
└── favicon/                # OneMark branded icons
    ├── favicon.ico
    └── site.webmanifest

```

---

## 🚀 Getting Started

### Prerequisites

* A modern web browser.

### 1. Clone the repository

```bash
git clone https://github.com/viswabnath/ea-wedding-counter.git
cd ea-wedding-counter

```

### 2. Run Locally

Because the external Firebase dependencies have been removed, you can now simply **double-click `index.html**` or open it directly in any modern browser to view the project.

---

## 🎨 Customization

### Updating the Wedding Date

Open `index.html` and find the `WEDDING` constant in the script tag to adjust the target timestamp:

```javascript
const WEDDING = new Date("February 15, 2025 10:54:00 GMT+0530").getTime();

```

### Changing the Theme Colors

The colors are defined in CSS variables at the top of the `<style>` block:

```css
:root {
    --color-red: #b83c3c;   /* Royal Red */
    --color-gold: #c59d5f;  /* Elegant Gold */
}

```

---

## 🛡️ Static Transition Note

This project has been intentionally stripped of its Firebase and Netlify backend dependencies to ensure the site remains a fast, permanent, and offline-capable static archive. The "Happily Married" status is now the permanent landing experience for all visitors.

---

[![Live Site](https://img.shields.io/badge/🌐%20View%20Live%20Site-EA%20Wedding%20Counter-B83C3C?style=for-the-badge&logoColor=white)](https://anil-eswari.netlify.app)

## 💛 Credits

Designed with ❤️ for **#EAParinayam** by [OneMark](https://onemark.co.in).
