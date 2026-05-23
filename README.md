# 🎬 RNDb - The Ultimate Movie & TV Show Database

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)](https://getbootstrap.com/)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com/)
[![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://vercel.com/)

A premium, serverless Movie and TV Show discovery web application built using native **Vanilla web technologies (HTML/CSS/JS)**, styled beautifully with **Bootstrap 5**, powered by the **TMDb API** for rich real-time media data, and backed by **Google Firebase** for secure user authentication and cloud synchronization of watchlists and reviews.

---

## ✨ Features

- **🌐 Dynamic Discovery:** Real-time trending movies, TV shows, and celebrities fetched directly from **The Movie Database (TMDb)** API.
- **🔍 Deep Search & Filters:** Search for any movie, TV show, or actor with clean, paginated results and comprehensive details.
- **🔐 Firebase Authentication:** Secure user registration, login, and Google OAuth login to manage personalized accounts.
- **📂 Cloud Watchlist:** Add movies/shows to a personalized Watchlist, synced instantly to **Cloud Firestore** and cached locally via `localStorage` for instant performance.
- **✍️ User Reviews System:** Write reviews, rate films, and view reviews left by other users with dynamic sorting and paginated list views.
- **📋 Custom Movie Lists:** Create, edit, and share customized collections of your favorite movies directly from your user profile.
- **🎨 Sleek Dark Aesthetic:** Modern dark theme styling, subtle glassmorphism effects (`backdrop-filter`), hardware-accelerated micro-animations, and fluid transitions.

---

## 🛠️ Tech Stack & Architecture

### Frontend
- **HTML5:** Modular multi-page architecture separating specific views (`index.html`, `detail.html`, `profile.html`, etc.) for faster initial loads and excellent SEO structure.
- **Vanilla JavaScript (ES6+):** Pure, native JS handling DOM manipulation, event listeners, and API network requests without heavy frameworks.
- **Bootstrap 5.3.3:** Responsive grid system, custom dark-mode styling, Modals, Toasts, Dropdowns, and components.
- **CSS3 & Google Fonts:** Sleek custom CSS (`style.css`) using CSS variables, custom themes (`--rndb-yellow`), and typography featuring the *Inter* font family.

### Backend & Database (Serverless)
- **Firebase Authentication:** Handles user identities securely.
- **Cloud Firestore:** NoSQL database storing user profiles, user-generated reviews, and custom watchlists.
- **TMDb API:** Real-time data engine serving posters, casting details, trailers, and overview details.

---

## 🚀 How to Run Locally

Since this is a lightweight, frontend-first project, running it locally is incredibly simple:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/NitinChamp1/rndb.git
   cd rndb
   ```

2. **Open the Project:**
   Simply open the `public/index.html` file directly in any modern browser, or run a local development server for the best experience:
   - If you have VS Code, use the **Live Server** extension.
   - Or, run using Python in your terminal:
     ```bash
     python -m http.server 8000
     ```
     *Then open `http://localhost:8000/public/` in your browser.*

---

## 📦 Deployment

### Vercel
This project is configured to deploy instantly to Vercel via the `vercel.json` file, which automatically handles routing for the multi-page application structure.

### Firebase
With the built-in `firebase.json` and `.firebaserc` setup, you can deploy static assets to Firebase Hosting with a single command:
```bash
firebase deploy
```
