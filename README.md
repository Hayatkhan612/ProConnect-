# 🦅 ProConnect Messenger - Ultra Secured Edition

**ProConnect** is a professional-grade, real-time messaging platform architected for "Blue Team" defense. This "Ultra-Secured" version implements enterprise-level security protocols, including client-side end-to-end encryption and a modular security management system.

> **Hacker's Note:** This entire project was developed on a **mobile device (4GB RAM)**, proving that high-security software doesn't require high-end hardware.

---

## 🛡️ "Fort Knox" Security Architecture
Unlike standard messaging apps, ProConnect utilizes a custom-built **SecurityManager** class to handle all defensive operations:

* **End-to-End Encryption (E2EE)**: Messages are encrypted with **AES-256** using CryptoJS before they leave the device. Even the database only sees scrambled ciphertext.
* **Brute Force Defense**: Implements an automatic account lockout system after 5 failed attempts with a 15-minute cooldown period.
* **Intelligent Rate Limiting**: Throttles user requests (max 30 per minute) to mitigate spam and potential DDoS vectors.
* **Advanced XSS & CSRF Protection**: All inputs are sanitized through a manual sanitization engine, and unique session tokens validate every state-changing request.
* **Security Watermark**: A persistent UI indicator verifies the active ultra-secured status of the session.

---

## 🚀 Key Features
* **Encrypted Real-time Chat**: Instant delivery via Firebase Firestore with zero-knowledge storage.
* **WebRTC Voice & Video**: Secure, peer-to-peer communication using DTLS-SRTP for media encryption.
* **Smart Presence**: Securely tracks online/offline status and "Typing..." indicators without exposing user metadata.
* **Security Dash (Admin)**: Hidden dashboard for authorized UIDs to monitor system-wide security metrics.
* **Lean & Fast**: Optimized SVG architecture for low-memory (4GB RAM) mobile environments.

---

## 🛠️ Tech Stack & Defense Tools
* **Encryption**: AES-256 (CryptoJS).
* **Frontend**: React 18 (UMD), Tailwind CSS.
* **Backend**: Firebase v9 (Auth, Firestore, Storage) with strictly hardened **Firestore Security Rules**.
* **Environment**: Mobile-First Production Sprint.

---

## 📦 Installation & Audit
1. View the live production app: [hayatkhan612.github.io/ProConnect-/](https://hayatkhan612.github.io/ProConnect-/)
2. To audit the code locally:
   ```bash
   git clone [https://github.com/hayatkhan612/ProConnect-.git](https://github.com/hayatkhan612/ProConnect-.git)
