# Mentee Connection Tracker

A simple, beautiful web app to help mentors track and manage regular check-ins with their mentees.

![License](https://img.shields.io/badge/license-MIT-blue.svg)

## 🎯 Features

- **Smart Priority Queue** - Color-coded system shows who needs contact (Red: 14+ days, Yellow: 7-13 days, Green: recent)
- **Quick Logging** - One-tap buttons to log texts and calls with automatic timestamps
- **Interaction History** - Complete timeline of all contacts with each mentee
- **Personal Notes** - Add and edit notes for each mentee (goals, interests, updates)
- **Weekly Stats** - Track your mentor engagement at a glance
- **Search & Filter** - Quickly find mentees by name or specialty
- **Data Backup** - Export and import your data as JSON
- **100% Private** - All data stored locally in your browser (LocalStorage)
- **Mobile-First Design** - Works beautifully on phones and tablets
- **No Installation** - Just open in any browser

## 🚀 Quick Start

### Option 1: Use It Online (Recommended)
1. Visit the deployed app: `https://yourusername.github.io/mentee-tracker`
2. Bookmark it on your phone's home screen
3. Start tracking your mentees!

### Option 2: Run Locally
1. Download `index.html`
2. Double-click to open in your browser
3. That's it!

## 📱 Add to iPhone Home Screen

1. Open the app in Safari
2. Tap the Share button (square with arrow)
3. Scroll down and tap "Add to Home Screen"
4. Now it works like a native app!

## 🛠️ Deployment to GitHub Pages

### Step 1: Create Repository
```bash
cd mentee-tracker
git init
git add .
git commit -m "Initial commit: Mentee Connection Tracker"
```

### Step 2: Push to GitHub
```bash
# Create a new repo on GitHub first, then:
git remote add origin https://github.com/yourusername/mentee-tracker.git
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages
1. Go to your repo on GitHub
2. Click **Settings** > **Pages**
3. Under "Source", select **main** branch
4. Click **Save**
5. Your app will be live at: `https://yourusername.github.io/mentee-tracker`

## 💾 Data Management

### Your Data is Safe
- All data is stored locally in your browser's LocalStorage
- No data is sent to any server
- Maximum privacy and security

### Backup Your Data
1. Click the **"Export Data"** button
2. Save the JSON file somewhere safe (Google Drive, Dropbox, etc.)
3. You can import this file later to restore your data

### Import Data
1. Click **"Import Data"**
2. Select your previously exported JSON file
3. Your data will be restored

## 🎨 Customization

The app uses a single HTML file with inline CSS and JavaScript. To customize:

1. Open `index.html` in any text editor
2. Find the `<style>` section to modify colors and layout
3. Find the `<script>` section to modify functionality
4. Save and refresh your browser

### Quick Customizations

**Change Priority Thresholds:**
```javascript
// In the getDaysAgo() function, modify these values:
if (days >= 14) return { color: 'red', label: days + ' days ago' };
if (days >= 7) return { color: 'yellow', label: days + ' days ago' };
```

**Add More Specialties:**
```javascript
// In the generateFakeMentees() function:
const specialties = ['Cardiology', 'Neurology', 'Your New Specialty'];
```

## 📊 Technical Details

- **Pure Vanilla JavaScript** - No frameworks, no build process
- **LocalStorage API** - Persistent data without a backend
- **Mobile-First CSS** - Responsive design using Flexbox
- **Single File** - Everything in one HTML file (~600 lines)
- **No Dependencies** - Works completely offline

## 🤝 Use Cases

Perfect for:
- Medical residents/fellows mentoring students
- Academic advisors tracking student check-ins
- Managers maintaining team relationships
- Anyone managing regular 1-on-1 connections

## 🔒 Privacy

- **No tracking**: No analytics, no cookies, no external scripts
- **No server**: Runs entirely in your browser
- **No account**: No login required
- **Your data stays yours**: Everything stored locally

## 📝 License

MIT License - feel free to modify and use for any purpose!

## 🐛 Troubleshooting

**Data disappeared?**
- LocalStorage can be cleared if you clear browser cache
- Always keep regular exports of your data
- Consider bookmarking the app to prevent accidental clearing

**Not working on phone?**
- Make sure JavaScript is enabled in your browser
- Try Safari or Chrome (recommended)
- Check that you have enough storage space

**Need to reset everything?**
- Open browser console (F12)
- Type: `localStorage.clear()` and press Enter
- Refresh the page

## 🎓 Educational Use

This project is perfect for:
- Learning vanilla JavaScript
- Understanding LocalStorage
- Practicing mobile-first design
- Demonstrating rapid prototyping
- Teaching web development basics

## ⭐ Contributing

This is a personal project, but suggestions are welcome! 
- Fork the repo
- Make your changes
- Submit a pull request

---

Built with ❤️ for mentors who care about staying connected.

