# Wedding Countdown

This is a simple countdown timer for Anil & Eswari's wedding, featuring a live visitor counter. The website displays a festive countdown to the big day, accompanied by an elegant design and smooth animations.

## Features:
- **Countdown Timer**: A dynamic countdown to the wedding day with days, hours, minutes, and seconds.
- **Visitor Counter**: Tracks the number of visitors to the page using Firebase Realtime Database.
- **Responsive Design**: Optimized for all screen sizes (desktop, tablet, mobile).
- **Hover Effects**: Background brightness and container shadow effects on hover for a dynamic feel.

## Technologies Used:
- **HTML** for structuring the content
- **CSS** for styling the page (responsive and interactive effects)
- **JavaScript** for the countdown timer and visitor counter functionality
- **Firebase** for the live visitor counter

## Getting Started

### Prerequisites:
Make sure you have an internet connection as this project relies on Firebase for the visitor counter.

### Steps to Run Locally:
1. Clone the repository or download the files.
   ```bash
   git clone https://github.com/yourusername/ea-wedding-counter.git

### To make the visitor counter work with Firebase, you will need to:

2. Go to the Firebase Console.
Create a new Firebase project (or use an existing one).
Set up the Firebase Realtime Database and get your project's Firebase configuration.
Replace the firebaseConfig object in the index.html file with your Firebase project's configuration.

const firebaseConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_AUTH_DOMAIN",
    databaseURL: "YOUR_DATABASE_URL",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_STORAGE_BUCKET",
    messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
    appId: "YOUR_APP_ID",
    measurementId: "YOUR_MEASUREMENT_ID"
};

### How to Use:
1. **Clone the repository** (or copy the files) to your local machine.
2. **Set up Firebase**: Ensure you configure Firebase in the `firebaseConfig` section.
3. **Open in browser**: Simply open the `index.html` file in any modern browser.

### To Contribute:
Feel free to submit issues or pull requests for bugs, improvements, or features.

Let me know if you need any adjustments!
