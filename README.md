Snap & Shop: AI Fashion Finder

📌 Project Overview
Snap & Shop is a mobile application built using **React Native (Expo Framework)** that allows users to capture outfit images and find similar clothing items online. The app enhances user experience through **image manipulation, networking, and location-based services**, providing a seamless shopping experience.

🎯 Features
- **Outfit Image Capture** – Take a picture of an outfit using the device camera.
- **AI-based Image Analysis** – Process images to identify outfit details.
- **Product Search & Recommendations** – Fetch similar clothing items from an online database.
- **User Authentication & Profile Management** – Register, log in, and edit profiles with profile image manipulation.
- **Location-Based Services** – Recommend nearby stores selling similar products.
- **Offline Data Storage** – Store user preferences and past searches using SQLite.
- **User-Friendly UI/UX** – Intuitive design with animations and optimized layouts.
- **Firebase Backend** – Authentication, real-time database, and cloud storage integration.

🚀 Installation & Setup
 Prerequisites
Ensure you have the following installed:
- **Node.js** (Latest LTS Version)
- **Expo CLI** (`npm install -g expo-cli`)
- **Android Studio/Xcode** (for emulator testing)
- **Firebase SDK** (for authentication and real-time database)

 Install Dependencies
```sh
npm install
```

 Configure Firebase
1. Create a Firebase project at [Firebase Console](https://console.firebase.google.com/).
2. Enable **Authentication**, **Firestore Database**, and **Storage**.
3. Download the `google-services.json` (for Android) and `GoogleService-Info.plist` (for iOS) and place them in the appropriate directories.
4. Install Firebase dependencies:
   ```sh
   npm install firebase
   ```
5. Configure Firebase in `firebase.jsx`.

### Start the Expo Development Server
```sh
expo start
```
Scan the QR code with your Expo Go app to preview the application on your mobile device.

 📁 Project Structure
```
snapshop/
│-- node_modules/
│-- assets/
│-- constants/
│-- hooks/
│-- scripts/
│-- android/
│-- app/
│   │-- login/
│   │   │-- LoginScreen.jsx
│   │   │-- SignUpScreen.jsx
│   │-- screens/
│   │   │-- BillingScreen.jsx
│   │   │-- CartScreen.jsx
│   │   │-- CheckoutScreen.jsx
│   │   │-- FashionNewsScreen.jsx
│   │   │-- HomeScreen.jsx
│   │   │-- ImageEditorScreen.jsx
│   │   │-- LocationScreen.jsx
│   │   │-- ShopScreen.jsx
│   │   │-- WelcomeScreen.jsx
│   │-- _layout.tsx
│   │-- firebase.jsx
│-- .gitignore
│-- app.json
│-- eas.json
│-- expo-env.d.ts
│-- index.js
│-- metro.config.js
```

 📍 Key Functionalities & Implementation
 1️⃣ **User Authentication & Profile Management**
- Firebase authentication for secure login.
- Profile image manipulation (cropping, resizing, filtering).

 2️⃣ **Outfit Capture & Processing**
- Uses device camera to capture outfits.
- Image preprocessing for AI-based outfit analysis.

 3️⃣ **Networking & Product Search**
- Integrates with an external API or product database.
- Displays recommended clothing items based on AI analysis.

 4️⃣ **Location-Based Store Suggestions**
- Fetches nearby stores selling similar products.
- Displays store details (ratings, availability, distance).

 5️⃣ **Database Integration for Offline Mode**
- Firebase Firestore for real-time data synchronization.
- SQLite stores user preferences and past searches for offline access.
