# Хөвсгөл Хүргэлт - School Delivery Prototype

A simple delivery connection platform for Huvsgul area.

## 🚀 Quick Setup

### 1. Firebase Setup

1. Go to [Firebase Console](https://console.firebase.google.com/)
2. Create a new project
3. Click on "Realtime Database" and create a database
4. Set rules to:
```json
{
  "rules": {
    "carriers": {
      ".read": true,
      ".write": true
    }
  }
}
```
5. Go to Project Settings → General → Your apps
6. Click "Web" and register your app
7. Copy the Firebase config object

### 2. Update Firebase Config

Replace the Firebase configuration in **both** `signup.html` and `carriers.html`:

```javascript
const firebaseConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
    databaseURL: "https://YOUR_PROJECT_ID.firebaseio.com",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_PROJECT_ID.appspot.com",
    messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
    appId: "YOUR_APP_ID"
};
```

### 3. Deploy to Vercel

1. Push your code to GitHub
2. Go to [Vercel](https://vercel.com)
3. Click "New Project"
4. Import your GitHub repository
5. Click "Deploy"

That's it! Your site will be live.

## 📁 File Structure

```
├── index.html          # Main menu
├── signup.html         # Carrier signup page
├── carriers.html       # View all carriers
├── style.css          # Styling
└── README.md          # This file
```

## ✨ Features

- ✅ Carrier registration with phone & description
- ✅ PIN-protected edit/delete
- ✅ Real-time updates
- ✅ Mobile responsive design
- ✅ Clean, modern UI

## 🛠️ Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- Firebase Realtime Database

---

**School Project • Prototype**
