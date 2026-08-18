# 🚀 Karel Playground - Progressive Web App (PWA)

An interactive Karel programming playground for learning algorithms and computational thinking concepts. Built as a Progressive Web App (PWA) that can be installed on any device.

---

## 🌐 Live Demo
Access the live interactive application on GitHub Pages:  
👉 **[https://andrewtliem.github.io/karel-mice/](https://andrewtliem.github.io/karel-mice/)**

---

## 🧩 Computational Thinking dengan Karel Playground

| Pilar CT | Penerapan Praktis di Karel Playground |
| :--- | :--- |
| **1. Decomposition** | Mahasiswa memecah tugas besar (misal: *Menyelesaikan Labirin*) menjadi sub-fungsi modular:<br>• `function turn_right() { turn_left(); turn_left(); turn_left(); }`<br>• `function solve_step() { ... }` |
| **2. Pattern Recognition** | Mahasiswa melihat pola labirin berulang dan menyusun perulangan (*loop*):<br>• *"Selama depan kosong, maju terus"* &rarr; `while (front_is_clear()) { move(); }` |
| **3. Abstraction** | Mahasiswa menggunakan sensor kondisi tingkat tinggi (`front_is_clear()`, `balls_present()`) tanpa perlu memikirkan perhitungan koordinat piksel layar yang rumit. |
| **4. Algorithm Thinking** | Mahasiswa merancang algoritma navigasi sederhana seperti **Wall Follower (Aturan Tangan Kanan/Kiri)** untuk keluar dari labirin. |

---

## ✨ Features

- **Interactive Karel Robot**: Visual programming with a cute dog/cat/mouse robot
- **Real-time Code Execution**: Write JavaScript code and see Karel move in real-time
- **World Builder**: Create custom mazes and worlds
- **Step-by-step Execution**: Debug your code with step-by-step animation
- **Smart Karel Tool**: Click to place, double-click to rotate, right-click to rotate
- **Save/Load Projects**: Save both world layout and code together
- **Offline Support**: Works without internet connection
- **Installable**: Add to home screen like a native app
- **Responsive Design**: Works on desktop, tablet, and mobile

---

## 🎯 PWA Features

- ✅ **Installable** - Add to home screen
- ✅ **Offline Support** - Works without internet
- ✅ **App-like Experience** - Full-screen mode
- ✅ **Fast Loading** - Cached resources
- ✅ **Cross-platform** - Works on all devices

---

## 🚀 Quick Start

### Option 1: Use Online Demo
Visit the live demo:  
👉 **[https://andrewtliem.github.io/karel-mice/](https://andrewtliem.github.io/karel-mice/)**

### Option 2: Run Locally
1. Clone this repository:
   ```bash
   git clone https://github.com/andrewtliem/karel-mice.git
   cd karel-mice
   ```
2. Open `index.html` in a web browser
3. Start programming with Karel!

---

## 📱 Installation

### Desktop / Chrome
1. Visit the app in Chrome
2. Click the install icon in the address bar (or click "📱 Install App" button in header)
3. Click "Install"

### Mobile (iOS)
1. Open in Safari
2. Tap the share button
3. Tap "Add to Home Screen"

### Mobile (Android)
1. Open in Chrome
2. Tap the menu (⋮)
3. Tap "Add to Home Screen"

---

## 🎮 How to Use

### Basic Commands
```javascript
move();           // Move forward one step
turn_left();      // Turn 90° left
put_ball();       // Place a ball
take_ball();      // Pick up a ball
```

### Control Flow
```javascript
if (front_is_clear()) {
  move();
} else {
  turn_left();
}

while (balls_present()) {
  take_ball();
  move();
  put_ball();
}
```

### World Building
1. Click "World Builder" button
2. Choose grid size and preset
3. Use tools to place balls, walls, and Karel
   - **Karel Tool**: Click to place/move Karel, double-click to rotate direction, right-click to rotate
4. Save your world for later use

---

## 🛠️ Project Structure
```
├── index.html          # Main application & Code editor
├── manifest.json       # PWA manifest
├── sw.js              # Service worker (Offline cache)
├── icons/             # App icons
└── README.md          # Documentation
```

### Technologies Used
- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Graphics**: HTML5 Canvas API
- **PWA**: Service Workers, Web App Manifest
- **Styling**: CSS Grid, Flexbox, CSS Variables

---

## 🌐 GitHub Pages Deployment

### Step 1: Push Repository
```bash
git clone https://github.com/andrewtliem/karel-mice.git
cd karel-mice
git add .
git commit -m "Update Karel Playground PWA"
git push origin main
```

### Step 2: Enable GitHub Pages
1. Go to repository on GitHub: [https://github.com/andrewtliem/karel-mice](https://github.com/andrewtliem/karel-mice)
2. Click **Settings** tab
3. Navigate to **Pages** section
4. Under **Source**, select `Deploy from a branch`
5. Choose `main` branch and `/ (root)` folder
6. Click **Save**

Your PWA will be live at:
```
https://andrewtliem.github.io/karel-mice/
```

---

## 📄 License
This project is open source and available under the [MIT License](LICENSE).

---

**Happy Programming! 🎉**  
*Built with ❤️ for students learning computational thinking & algorithms*
