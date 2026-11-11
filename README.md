# Vaakku — Privacy Policy & GitHub Pages Hosting Guide

This directory (`privacy-policy/`) contains the complete, Google Play Store and GDPR compliant Privacy Policy website for **Vaakku (വാക്ക്)**, built ready to be hosted with zero cost using **GitHub Pages**.

---

## 📁 Files Included

| File | Purpose |
|---|---|
| `index.html` | Responsive, modern HTML5 website with full legal disclosures, Google Play Data Safety matrix, and bilingual (English + Malayalam) summaries. |
| `style.css` | Styled with Vaakku's brand identity (Backwater Green `#0E5A4B` & Kasavu Gold `#C9962F`), dark mode support, and print stylesheet. |
| `.nojekyll` | Ensures GitHub Pages bypasses Jekyll static analysis and serves all files directly. |

*(A synchronized copy is also placed in `docs/` and `docs/privacy-policy/` so whichever folder you choose in GitHub Pages settings will work instantly.)*

---

## 🚀 How to Host on GitHub Pages (Step-by-Step)

### Step 1: Push the Changes to GitHub
Commit and push the new files to your repository:
```bash
git add privacy-policy/ docs/
git commit -m "Add Privacy Policy page for GitHub Pages"
git push origin main
```

### Step 2: Enable GitHub Pages in Repository Settings
1. Open your repository on GitHub (`https://github.com/<your-username>/<your-repo>`).
2. Click on **Settings** (tab at the top right).
3. In the left sidebar, under **Code and automation**, click **Pages**.
4. Under **Build and deployment**:
   - **Source**: Select `Deploy from a branch`.
   - **Branch**: Select `main` (or `master`).
   - **Folder**:
     - **Option A (Recommended)**: Select `/ (root)`.
       Your URL will be:
       `https://<your-username>.github.io/<your-repo>/privacy-policy/`
     - **Option B**: Select `/docs`.
       Your URL will be:
       `https://<your-username>.github.io/<your-repo>/` (or `/privacy-policy/`)
5. Click **Save**.

### Step 3: Access Your Live Privacy Policy
Within 1–2 minutes, GitHub will build and publish your site. You will see a green banner stating:
> *"Your site is live at `https://<your-username>.github.io/<your-repo>/privacy-policy/`"*

---

## 📲 How to Add to Google Play Console

Google Play requires a working public Privacy Policy URL before you can publish or update your app bundle:

1. Log in to the [Google Play Console](https://play.google.com/console).
2. Select your app: **Vaakku**.
3. In the left navigation menu, scroll down to **Policy and programs** → **App content**.
4. Under **Privacy Policy**, click **Start** (or **Manage**).
5. Paste your live GitHub Pages URL:
   ```
   https://<your-username>.github.io/<your-repo>/privacy-policy/
   ```
6. Click **Save**.

---

## 🛡️ Play Console Data Safety Form Reference

The page includes a dedicated **Google Play Data Safety Matrix** matching the libraries used in this codebase:
- **Firebase Authentication**: User email & user ID (Optional, only for users who sign in with Google).
- **Firebase Firestore**: Weekly leaderboard points & display name.
- **Google AdMob**: Device ID, Advertising ID (AAID/GAID), coarse location from IP, and diagnostic interaction metrics.
- **Firebase Analytics**: Aggregated session counts and app engagement metrics.
- **Data Encryption**: All data in transit is encrypted using HTTPS / TLS.
- **Data Deletion**: Users can clear local data via App settings, or email support for cloud deletion.

