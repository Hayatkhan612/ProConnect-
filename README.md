# 🦅 ProConnect Messenger

**ProConnect** is a secure, professional-grade real-time messaging web application. Built with a focus on high performance and "Blue Team" defense, it is designed to run efficiently on mobile devices with limited resources (4GB RAM) without sacrificing security.

---

## 🛡️ Security Audit & "Hacker" Mindset
As a developer with a background in cybersecurity, I built ProConnect with a **Security-First** approach. Unlike standard "Test Mode" apps, ProConnect features:

* **Custom Firestore Security Rules**: Granular access control prevents unauthorized database wipes or data snooping.
* **Packet Isolation**: Users can only read or write to chat rooms where their `UID` is explicitly listed in the `participants` array.
* **Identity Guard**: Only authenticated owners can modify their profile metadata (Email/UID/ShareCode).
* **XSS Mitigation**: Leverages React's built-in sanitization to prevent stored XSS attacks via chat inputs.

---

## 🚀 Features
* **Email Discovery**: Find and add friends directly via their professional email address.
* **Real-time Communication**: Instant message delivery powered by Firebase Firestore `onSnapshot` listeners.
* **Lean Architecture**: Zero external image dependencies. Uses SVG icons and the UI-Avatars API to save bandwidth and device memory.
* **Native Share Integration**: Uses the Web Share API for a seamless mobile "Invite Friend" experience.
* **Mobile Optimized**: Responsive design that toggles between sidebar and chat views for a native-app feel.

---

## 🛠️ Tech Stack
* **Frontend**: React 18 (UMD), Tailwind CSS
* **Backend**: Firebase v9 (Auth, Firestore)
* **Language**: JavaScript (ES6+)
* **Environment**: Mobile-First Development

---

## 📦 Installation & Setup
1. Clone the repository:
   ```bash
   git clone [https://hayatkhan612.github.io/ProConnect-/](https://hayatkhan612.github.io/ProConnect-/)
