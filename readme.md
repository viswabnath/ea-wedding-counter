
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
├── index.html              # Main application file (Contains Firebase Config)
├── background.jpg          # Couple background photo (Royal Theme)
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
3. Enable **Realtime Database**.
4. Set the Rules to allow public reads/writes (or use the secure increment-only rules found below).
5. Copy your project's configuration keys.

### 3. Configure `index.html`

Open `index.html` and scroll to the bottom script section. Replace the placeholder values in `firebaseConfig` with your actual keys:

```javascript
const firebaseConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_PROJECT.firebaseapp.com",
    databaseURL: "https://YOUR_PROJECT.firebaseio.com",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_PROJECT.appspot.com",
    messagingSenderId: "YOUR_SENDER_ID",
    appId: "YOUR_APP_ID",
    measurementId: "YOUR_MEASUREMENT_ID"
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
4. Your site will be live immediately.

> **Note on Security:** Since this is a static site, Firebase keys are public. To secure your data, ensure your Firebase Realtime Database **Rules** are set to only allow valid visitor increments, preventing anyone from deleting or overwriting your data.

---

## 🤝 Contributing

Feel free to submit issues or pull requests for bugs, improvements, or new features.

---

## 💛 Credits

Designed with ❤️ for **#EAParinayam** by [OneMark]().
