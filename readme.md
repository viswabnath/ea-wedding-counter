
# 💍 Anil & Eswari's Wedding Countdown — #EAParinayam

> A royal, animated wedding countdown page designed for Anil & Eswari's big day.

[![Live Site](https://img.shields.io/badge/🌐%20View%20Live%20Site-EA%20Wedding%20Counter-B83C3C?style=for-the-badge&logoColor=white)](https://viswabnath.github.io/ea-wedding-counter/)
[![Made with Love](https://img.shields.io/badge/Made%20with-❤️-B83C3C?style=for-the-badge)](https://onemark.co.in)
[![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-222222?style=for-the-badge&logo=github&logoColor=white)](https://viswabnath.github.io/ea-wedding-counter/)

---

## ✨ Features

- **👑 Royal Aesthetics** — Designed with a luxurious **Red & Gold** theme, featuring *Great Vibes* (script) and *Cinzel* (royal serif) fonts.
- **📱 Smart Mobile Layout** — The layout is anchored to the bottom of the screen on mobile devices, ensuring the couple's faces in the background photo remain perfectly visible.
- **⏳ Floating Countdown** — The countdown timer floats elegantly *outside* the main glass card, creating a modern, layered depth effect.
- **🌸 Floating Petal Animation** — Gentle red & pink petals drift across the background for a festive, romantic touch.
- **👀 Live Visitor Counter** — Tracks real-time visitors using Firebase Realtime Database, shown with a pulsing "live" indicator.
- **🎨 Glassmorphism UI** — Features a frosted glass effect (`backdrop-filter: blur`) that ensures text readability over the photo.
- **🔒 Secure Config** — Firebase credentials are loaded from a gitignored `env.js` file, keeping secrets safe.

---

## 🛠 Technologies Used

| Layer      | Technology |
|------------|------------|
| Structure  | HTML5 |
| Styling    | CSS3 (Flexbox, `clamp()`, Glassmorphism, Animations) |
| Fonts      | Google Fonts — **Cinzel** (Headers), **Great Vibes** (Names), **Montserrat** (Body) |
| Logic      | Vanilla JavaScript (ES Modules) |
| Database   | Firebase Realtime Database (Visitor Counter) |
| Hosting    | GitHub Pages |

---

## 📁 Project Structure

```text
ea-wedding-counter/
├── index.html              # Main application file
├── background.JPG          # Couple background photo (Royal Theme)
├── env.js                  # 🔒 Firebase secrets — gitignored
├── README.md               # Project documentation
└── favicon/                # OneMark branded icons
    ├── favicon.ico
    ├── favicon-96x96.png
    ├── favicon.svg
    ├── apple-touch-icon.png
    └── site.webmanifest

```

---

## 🚀 Getting Started

### Prerequisites

* A modern browser.
* A Firebase project with Realtime Database enabled.
* A local server (since the project uses ES Modules).

### 1. Clone the repository

```bash
git clone [https://github.com/viswabnath/ea-wedding-counter.git](https://github.com/viswabnath/ea-wedding-counter.git)
cd ea-wedding-counter

```

### 2. Set up Firebase

1. Go to the [Firebase Console]().
2. Create a new project.
3. Enable **Realtime Database** and set rules to `read: true, write: true` (for testing).
4. Copy your project's configuration keys.

### 3. Configure your secrets

Create an `env.js` file in the root directory (**this file is gitignored**):

```javascript
// env.js — DO NOT COMMIT THIS FILE
window.__ENV = {
  FIREBASE_API_KEY:             "YOUR_API_KEY",
  FIREBASE_AUTH_DOMAIN:         "YOUR_AUTH_DOMAIN",
  FIREBASE_DATABASE_URL:        "YOUR_DATABASE_URL",
  FIREBASE_PROJECT_ID:          "YOUR_PROJECT_ID",
  FIREBASE_STORAGE_BUCKET:      "YOUR_STORAGE_BUCKET",
  FIREBASE_MESSAGING_SENDER_ID: "YOUR_MESSAGING_SENDER_ID",
  FIREBASE_APP_ID:              "YOUR_APP_ID",
  FIREBASE_MEASUREMENT_ID:      "YOUR_MEASUREMENT_ID",
};

```

### 4. Run Locally

Because this project uses ES Modules (`type="module"`), you cannot simply double-click `index.html`. You must run it via a local server.

**Using Python:**

```bash
python3 -m http.server
# Then open http://localhost:8000

```

**Using Node (serve):**

```bash
npx serve .

```

---

## 🎨 Customization

### Updating the Wedding Date

Open `index.html` and find the `WEDDING` constant in the script tag:

```javascript
// Set the date to February 15, 2025
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

## 🌐 Deploying to GitHub Pages

1. Push your changes to the `main` branch.
2. Go to **Settings → Pages** in your repository.
3. Set the source to `main / root`.
4. **Important:** Since `env.js` is gitignored, you must manually upload/create the `env.js` file on your hosting server or inject the variables during a build process if using a pipeline. For simple GitHub Pages usage, you might need to commit `env.js` (warning: exposes API keys) or use a secure alternative layout.

---

## 🤝 Contributing

Feel free to submit issues or pull requests for bugs, improvements, or new features.

---

## 💛 Credits

Designed with ❤️ for **#EAParinayam** by [OneMark]().

