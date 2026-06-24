# BudgetFlow — Hosting & iPhone Installation Guide

## What you need to upload (5 files total)

Make sure you have all these files in one folder:
```
index.html        ← your dashboard (rename from expense-dashboard.html)
manifest.json     ← PWA config
sw.js             ← service worker (offline support)
icon-192.png      ← app icon
icon-512.png      ← app icon (large)
```

---

## Step 1 — Create a free GitHub account

1. Go to **https://github.com** and click **Sign up**
2. Choose a username, enter your email and a password
3. Verify your email address
4. You're in — this takes about 2 minutes

---

## Step 2 — Create a new repository

1. Click the **+** icon (top right) → **New repository**
2. Fill in:
   - **Repository name:** `budgetflow`
   - **Visibility:** ✅ Public  ← required for free GitHub Pages
   - Leave everything else as-is
3. Click **Create repository**

---

## Step 3 — Upload your files

1. On your new empty repo page, click **uploading an existing file** (the link in the middle of the page)
2. **Rename** `expense-dashboard.html` to `index.html` on your computer first
3. Drag all 5 files into the upload area:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
4. Scroll down, click **Commit changes**

---

## Step 4 — Enable GitHub Pages

1. Go to your repo's **Settings** tab (top menu)
2. Scroll down to **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Set branch to **main**, folder to **/ (root)**
5. Click **Save**
6. Wait ~60 seconds, then refresh the page
7. You'll see: *"Your site is live at https://yourusername.github.io/budgetflow"*

✅ **Your dashboard is now live on the internet!**

---

## Step 5 — Install on your iPhone

1. Open **Safari** on your iPhone (must be Safari, not Chrome)
2. Go to your URL: `https://yourusername.github.io/budgetflow`
3. Wait for the page to fully load
4. Tap the **Share button** (the box with an arrow pointing up ⬆️) at the bottom of the screen
5. Scroll down in the share sheet and tap **"Add to Home Screen"**
6. Change the name if you want (or leave it as BudgetFlow)
7. Tap **Add** in the top right

🎉 **BudgetFlow now appears on your iPhone home screen like a real app!**

---

## What works after installation

| Feature | Status |
|---|---|
| Full dashboard | ✅ Works |
| All data saved locally | ✅ Works (localStorage) |
| Works without internet | ✅ Works (cached offline) |
| 21:00 evening reminder | ✅ Works (while app is open) |
| Home screen icon | ✅ Works |
| No browser address bar | ✅ Full screen |
| Syncs between devices | ❌ Not yet (would need a backend) |

---

## Updating the dashboard in the future

When you get an updated `index.html` from Claude:
1. Go to your GitHub repo at `github.com/yourusername/budgetflow`
2. Click on `index.html` in the file list
3. Click the **pencil icon** (Edit) or **upload icon**
4. Replace the file with the new version
5. Click **Commit changes**
6. The live site updates within ~60 seconds automatically

---

## Troubleshooting

**"Site not found" after enabling Pages:**
→ Wait 2–3 minutes and hard-refresh the page

**The app doesn't go full screen on iPhone:**
→ Make sure you're using Safari (not Chrome) to add it

**Data disappeared:**
→ Your data lives in Safari's localStorage. Don't clear Safari website data for this site.

**Icon looks wrong on iPhone:**
→ Delete the app from your home screen and re-add it from Safari
