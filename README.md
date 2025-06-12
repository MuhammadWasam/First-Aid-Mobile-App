# Code Zip File Of First-Aid-Mobile-App

https://drive.google.com/file/d/1NEiXb3wGhtEmHvWNz6NC7ABPvx1dY0DY/view?usp=sharing

# Apk File Of First-Aid-Mobile-App

https://drive.google.com/file/d/1CQRDSI2jR0kJE8EKDj5qBH1O0lS7WP0u/view?usp=sharing

# 🩺 First Aid Mobile App (Expo + Laravel + Admin Panel)

This project is a full-stack mobile application consisting of:

- **FAid**: React Native frontend built with **Expo**
- **Backend**: Laravel PHP backend that serves API data
- **FAdmin**: Admin Panel (React/Vite) for uploading disease information 

---

## 📁 Project Structure

```
/FAdmin      → Admin Panel (React + Vite)
/Backend     → Laravel PHP backend (API and data)
/FAid        → React Native frontend (Expo mobile app)
```

---

## ⚙️ PART 1: Setting Up the Admin Panel (FAdmin)

### ✅ Prerequisites

- Node.js (https://nodejs.org/)

### ✅ Steps to Run

1. Open terminal and go to the `FAdmin` folder:

```bash
cd FAdmin
```

2. Install dependencies:

```bash
npm install
```

3. Start the development server:

```bash
npm run dev
```

4. Open the link shown in the terminal (usually `http://localhost:5173`)

---

## ⚙️ PART 2: Setting Up the PHP Backend (Laravel)

### ✅ Prerequisites

- PHP 8.x ([XAMPP](https://www.apachefriends.org/) or standalone)
- Composer (https://getcomposer.org/)
- MySQL 

### ✅ Steps to Run

1. Navigate to the `Backend` folder:

```bash
cd Backend
```

2. Install Laravel dependencies:

```bash
composer install
```

3. Copy `.env` and configure:

```bash
cp .env.example .env
```

Edit `.env` file:

```env
APP_URL=http://your-ip-address:8000
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database
DB_USERNAME=root
DB_PASSWORD=your_password
```

4. Generate app key:

```bash
php artisan key:generate
```

5. (Optional) Migrate database:

```bash
php artisan migrate
```

6. Start backend server:

```bash
php artisan serve --host=your-ip-address --port=8000
```

---

## 📱 PART 3: Setting Up the Mobile App (FAid with Expo)

### ✅ Prerequisites

- Node.js
- Expo CLI (`npm install -g expo-cli`)
- Android Studio (or Expo Go app on mobile)

### ✅ Steps to Run

1. Navigate to the `FAid` folder:

```bash
cd FAid
```

2. Install app dependencies:

```bash
npm install
```

3. Start Expo server:

```bash
expo start
```

4. Open the app:
   - Scan QR code with **Expo Go**
   - Or press `a` to open Android emulator

---

### ✅ Set Correct Backend URL

In FAid code, locate the API URL (likely in a Apiconfig.js in constants folder):

```js
const API_URL = "http://your-ip-address:8000/api";
```

Make sure it matches the Laravel server IP.

---

## 🌐 App Features

- 🔍 View first aid tutorials (steps + video + TTS)
- ✅ Symptom checker with animated results
- 📢 View emergency contacts and notifications
- 🔐 Admins upload diseases info via Admin Panel

---

## ✅ Common Commands

### Admin Panel

```bash
cd FAdmin
npm install
npm run dev
```

### Backend (Laravel)

```bash
cd Backend
composer install
cp .env.example .env
php artisan key:generate
php artisan serve --host=your-ip --port=8000
```

### Frontend (Expo)

```bash
cd FAid
npm install
expo start
```

---
