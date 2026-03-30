# 🚀 YLG Tracker Pro (PWA)

A high-performance, offline-first Progressive Web App (PWA) designed to track game profits, wallet balances, and referrals. Hosted on GitHub Pages with Google Sheets Cloud Sync.

## 🛠 Features
- **Offline Mode:** Save entries without internet; data stores locally on your phone.
- **Auto-Sync:** Automatically pushes data to Google Sheets when internet returns.
- **PWA Ready:** Install it on your home screen with custom icons.
- **Advanced Analytics:** Real-time Profit Trends (Line Chart) and Game Comparisons (Bar Chart).
- **Game Management:** Rename or delete game categories and all associated history.

## 📁 File Structure
- `index.html`: The main application code and logic.
- `manifest.json`: Configuration for app installation and icons.
- `service-worker.js`: Handles offline caching and automatic updates.
- `icon-192.png` & `icon-512.png`: Your custom app branding.

## 🔄 How to Update the App
Because this is a PWA, it saves a version on your phone for offline use. When you make changes to `index.html` on GitHub, follow these steps to ensure the update reaches your phone:

1. **Edit `index.html`**: Make your changes and commit.
2. **The Version Bump**: Open `service-worker.js`.
3. **Change the Version**: Change `const CACHE_NAME = 'ylg-v1';` to `v2`, `v3`, etc.
4. **Refresh**: The next time you open the app on your phone, a blue "New Update Available" bar will appear. Click **REFRESH** to apply the changes.

## ☁️ Cloud Sync Setup
The app is connected to a Google Sheet via a Web App URL. 
- **Upload**: Pushes your local phone data to the sheet.
- **Download**: Pulls data from the sheet (useful when switching devices).

---
*Built for professional tracking and data integrity.*
