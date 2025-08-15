# 🚀 Karel Playground - Progressive Web App

An interactive Karel programming playground for learning algorithms and programming concepts. Built as a Progressive Web App (PWA) that can be installed on any device.

## ✨ Features

- **Interactive Karel Robot**: Visual programming with a cute dog/cat robot
- **Real-time Code Execution**: Write JavaScript code and see Karel move in real-time
- **World Builder**: Create custom mazes and worlds
- **Step-by-step Execution**: Debug your code with step-by-step animation
- **Smart Karel Tool**: Click to place, double-click to rotate, right-click to rotate
- **Visual Direction Indicator**: See Karel's current direction when editing
- **Save/Load Projects**: Save both world layout and code together
- **Offline Support**: Works without internet connection
- **Installable**: Add to home screen like a native app
- **Responsive Design**: Works on desktop, tablet, and mobile

## 🎯 PWA Features

- ✅ **Installable** - Add to home screen
- ✅ **Offline Support** - Works without internet
- ✅ **App-like Experience** - Full-screen mode
- ✅ **Fast Loading** - Cached resources
- ✅ **Cross-platform** - Works on all devices

## 🚀 Quick Start

### Option 1: Use Online Demo
Visit the live demo: [https://andrewtliem.github.io/karel-mice/]

### Option 2: Run Locally
1. Clone this repository
2. Open `index.html` in a web browser
3. Start programming with Karel!

## 📱 Installation

### Desktop/Chrome
1. Visit the app in Chrome
2. Click the install icon in the address bar
3. Click "Install"

### Mobile (iOS)
1. Open in Safari
2. Tap the share button
3. Tap "Add to Home Screen"

### Mobile (Android)
1. Open in Chrome
2. Tap the menu (⋮)
3. Tap "Add to Home Screen"

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

## 🛠️ Development

### Project Structure
```
├── index.html          # Main application
├── manifest.json       # PWA manifest
├── sw.js              # Service worker
├── icons/             # App icons
└── README.md          # This file
```

### Technologies Used
- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Graphics**: HTML5 Canvas API
- **PWA**: Service Workers, Web App Manifest
- **Styling**: CSS Grid, Flexbox, CSS Variables

## 🌐 GitHub Pages Deployment

### Step 1: Create GitHub Repository
1. Go to [GitHub](https://github.com)
2. Click "New repository"
3. Name it: `karel-playground`
4. Make it public
5. Don't initialize with README (we already have one)

### Step 2: Upload Files
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/karel-playground.git
cd karel-playground

# Add all files
git add .

# Commit changes
git commit -m "Initial commit: Karel Playground PWA"

# Push to GitHub
git push origin main
```

### Step 3: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" section
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"

### Step 4: Access Your PWA
Your PWA will be available at:
```
https://YOUR_USERNAME.github.io/karel-playground/
```

## 🎨 Customization

### Colors
Edit CSS variables in `index.html`:
```css
:root {
  --accent: #3b82f6;      /* Primary blue */
  --accent-2: #06b6d4;    /* Secondary blue */
  --bg: #f8fafc;          /* Background */
  --panel: #ffffff;       /* Panel background */
}
```

### Icons
Replace placeholder icons in `icons/` folder with your own designs.

### World Presets
Add new world presets in the `presetWorld()` function.

## 🔧 Troubleshooting

### PWA Not Installing
- Ensure you're using HTTPS (GitHub Pages provides this)
- Check browser console for service worker errors
- Verify manifest.json is accessible

### Offline Not Working
- Check service worker registration in console
- Clear browser cache and reload
- Verify sw.js file is accessible

### Performance Issues
- Reduce grid size for complex worlds
- Use step-by-step execution for debugging
- Clear browser cache if needed

## 📚 Learning Resources

- **Karel Programming**: Learn basic programming concepts
- **JavaScript**: Modern ES6+ syntax
- **PWA Development**: Progressive Web App concepts
- **Canvas API**: 2D graphics programming

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Inspired by Karel the Robot programming language
- Built for educational purposes
- Uses modern web technologies for the best user experience

---

**Happy Programming! 🎉**

*Built with ❤️ for students learning to code*
