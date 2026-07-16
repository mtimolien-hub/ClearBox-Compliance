# ClearBoxCompliance.pro — Class II Medical Device Regulatory Pathway Decision Tree

Interactive regulatory decision tree for Class II medical device companies, covering **Hardware**, **AI/ML**, **SaMD**, and **SiMD** pathways.

## 🌐 Live Site
[https://ClearBoxCompliance.pro](https://ClearBoxCompliance.pro)

---

## 📁 Repository Structure

```
/
├── index.html      # Single-page interactive decision tree app
├── CNAME           # Custom domain mapping → ClearBoxCompliance.pro
├── .nojekyll       # Disables Jekyll processing (required for GitHub Pages)
└── README.md       # This file
```

---

## 🚀 Deployment Instructions

### 1. Create a GitHub Repository
- Go to [github.com](https://github.com) → **New repository**
- Name it exactly: `ClearBoxCompliance.pro` *(or any name — the CNAME handles domain routing)*
- Set visibility to **Public** (required for GitHub Pages on free plans)
- Do **not** initialize with a README (you already have one)

### 2. Push These Files
```bash
git init
git add .
git commit -m "Initial deploy: ClearBoxCompliance.pro decision tree"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

### 3. Enable GitHub Pages
1. In your repo → **Settings** → **Pages**
2. Under **Source**, select **Deploy from a branch**
3. Branch: `main` | Folder: `/ (root)`
4. Click **Save**
5. GitHub will display your deployment URL (e.g., `https://yourusername.github.io/repo-name`)

### 4. Configure Your Custom Domain (ClearBoxCompliance.pro)
The `CNAME` file in this repo is already set to `ClearBoxCompliance.pro`.

You must also add DNS records at your domain registrar:

| Type  | Host | Value                          | TTL  |
|-------|------|-------------------------------|------|
| A     | @    | 185.199.108.153                | 3600 |
| A     | @    | 185.199.109.153                | 3600 |
| A     | @    | 185.199.110.153                | 3600 |
| A     | @    | 185.199.111.153                | 3600 |
| CNAME | www  | YOUR_USERNAME.github.io        | 3600 |

> **Note:** DNS propagation can take up to 48 hours. GitHub will also auto-provision a free TLS/HTTPS certificate via Let's Encrypt once the domain resolves.

### 5. Enforce HTTPS
After the domain verifies → **Settings → Pages → Enforce HTTPS** ✅

---

## 🔧 Making Updates

To update the app, replace `index.html` with the new version and push:
```bash
git add index.html
git commit -m "Update decision tree: [describe change]"
git push
```
GitHub Pages redeploys automatically within ~60 seconds.

---

## ⚖️ Disclaimer
This application is for **informational purposes only** and does not constitute legal or regulatory advice. Consult qualified regulatory counsel for device-specific guidance.

© 2026 ClearBoxCompliance.pro — All rights reserved.
