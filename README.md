# 🌾 AgroSmart — Smart Soil Farming Platform

> Nurturing Growth & Vibrant Fields. Technology and farmer-first programs to enable productive, sustainable farming.

AgroSmart is a modern, responsive web application designed to empower farmers with **climate-smart data** and **actionable insights** for precise crop management. It provides real-time diagnostics, optimal resource usage recommendations, and a community network to boost yield and improve soil health sustainably.

## ✨ Features

* **Responsive Design:** Built using **Tailwind CSS** for a clean, mobile-first, and highly-customizable interface.
* **Firebase Authentication:** Secure user registration and login functionality using **Firebase Auth**.
* **Realtime Database Integration:** Stores new user profiles (Name, Email, Phone, Role) in the **Firebase Realtime Database**.
* **Role-Based Redirection:** Automatically directs users to `user-dashboard.html` and admins (via `admin@soilagent.com`) to `admin-dashboard.html` upon successful login.
* **Themed Aesthetics:** Uses a natural, soil-and-green color palette (`--primary-green`, `--soil-dark`) for an organic, inviting look.
* **Smooth Animations:** Implements basic JavaScript/Intersection Observer for "slide-up" animations as content comes into view.
* **Key Services:** Showcases core services like **Precision Zoning**, **Climate Resilience**, and **Farm-to-Market** support.

---

## 🛠️ Tech Stack

* **Frontend:** HTML5, Custom CSS, Vanilla JavaScript
* **Styling:** [Tailwind CSS](https://tailwindcss.com/) (via CDN)
* **Authentication & Database:** [Google Firebase](https://firebase.google.com/) (Auth and Realtime Database)
* **Fonts:** Quicksand & Open Sans (via Google Fonts CDN)

---

## 🚀 Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

You need a modern web browser and a Firebase project set up for the backend.

1.  **Firebase Project:** Create a project in the Firebase Console.
2.  **Enable Services:** Enable **Authentication** (Email/Password) and **Realtime Database** for the project.
3.  **Get Configuration:** Copy your Firebase project's configuration object.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your_username/agrosmart-platform.git](https://github.com/your_username/agrosmart-platform.git)
    cd agrosmart-platform
    ```
2.  **Add Assets:** The current HTML references images that are **not** included. Create an `img` folder in the root directory and place placeholders for the following files:
    * `/img/background.avif`
    * `/img/index-about.avif`
    * `/img/index-pic1.avif`
    * `/img/index-pic2.jpg`
    * `/img/index-pic3.avif`
    * `img/profile.jpg` (Used for community testimonials)
    *(Note: The page will still load without these, but the design will be incomplete.)*
3.  **Configure Firebase:** Open `index.html` and replace the placeholder `firebaseConfig` object in the `<script type="module">` section with your actual Firebase configuration details:

    ```javascript
    // Update this object with YOUR Firebase Project Credentials
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
    ```
4.  **Run:** Simply open the `index.html` file in your web browser.

---

## 💻 Usage & Testing

### User Accounts

* **Registration:** Click the **Register** button to open the modal. New users registered via this form will be created in Firebase Auth and saved to the Realtime Database under the `users/` path with the `role: "user"`.
* **User Login:** Log in with a standard registered user to be redirected to `user-dashboard.html`.
* **Admin Login:** Register a user with the specific email **`admin@soilagent.com`** in the Firebase Console. Logging in with this email will redirect you to `admin-dashboard.html`.

### Functionality

* **Contact Form:** The contact form is purely visual and uses a placeholder JS alert: `"Message sent! We'll contact you soon."`
* **Navigation:** The main navigation links point to placeholder files (`about.html`, `farmers.html`, `crops.html`) which need to be created.

---

## 🤝 Contributing

This is a front-end landing page template using embedded Firebase code. If you'd like to contribute by adding dashboard pages, improving styling, or implementing a proper build system (like Webpack/Vite for Tailwind), please feel free to fork the repository and open a Pull Request.

1.  Fork the project.
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the Branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.
---
# 📧 Contact

Project Link: [Click](https://vinayakgoyal2208.github.io/Soil-farming-agent/)




