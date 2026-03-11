# Wildlife and Fisheries Authorizations — Team Repository Hub

A GitHub Pages site that acts as a central hub for all BC Government Wildlife and Fisheries Authorizations team repositories.

**Live site:** _(once deployed — see instructions below)_

---

## ➕ How to Add a Repository

> **This is the only file you need to edit!**

1. Open **`repos.js`** in any text editor.
2. Copy an existing entry (the `{ … }` block) and paste it _before_ the closing `]`.
3. Make sure the previous entry ends with a **comma** `,`.
4. Fill in the four fields:

```js
{
  name: "My Repository",              // Display name on the card
  description: "What this does.",     // One sentence description
  url: "https://github.com/bcgov/…", // Full URL to the repository
  language: "Python"                  // Optional. Leave "" to hide badge.
                                      // Options: Python, R, JavaScript,
                                      //          TypeScript, SQL, Shell, Bash
}
```

5. **Save** the file.
6. **Commit and push** — the live site updates automatically (usually within 1–2 minutes).

---

## 🗑 How to Remove a Repository

Delete the `{ … }` block for the repository in `repos.js`. Make sure commas `,` between remaining entries are correct.

---

## 🚀 Deploying to GitHub Pages

### First-time setup

1. Create a new repository on GitHub (e.g., `fwa-team-hub`) under your org or personal account.
2. Push all files in this folder to the repository's `main` branch:

```bash
git init
git add .
git commit -m "Initial team hub site"
git remote add origin https://github.com/YOUR-ORG/fwa-team-hub.git
git push -u origin main
```

3. In GitHub, go to **Settings → Pages**.
4. Under **Source**, select **Deploy from a branch**.
5. Choose **Branch: `main`** and folder **`/ (root)`**.
6. Click **Save**. Your site will be live at:
   `https://YOUR-ORG.github.io/fwa-team-hub/`

### Updating the site

After edits, commit and push:

```bash
git add repos.js
git commit -m "Add new repository: <name>"
git push
```

GitHub Pages redeploys automatically — no build step required.

---

## 🖥 Local Preview

Open `index.html` directly in a browser (double-click the file). All features work without a local server.

---

## 📂 File Structure

```
fwa-team-hub/
├── index.html       # Main page (rarely needs editing)
├── style.css        # BC Gov-branded styles (rarely needs editing)
├── repos.js         # ← EDIT THIS FILE to add/remove repositories
├── assets/
│   └── hero.png     # Hero banner image (replace to update)
└── README.md        # This file
```

---

## 🎨 Design

- **Colours:** BC Government blue (`#234075`) and gold (`#E3A82B`)
- **Font:** BC Sans (loaded from the BC Government CDN)
- **Logo:** Official BC Mark loaded from the BC Government developer portal
- **Responsive:** Works on desktop, tablet, and mobile

---

## ✏️ Customization

| What to change | Where |
|---|---|
| Add/remove repos | `repos.js` |
| Team name or ministry | `index.html` — `<span class="header-team">` and `<span class="header-ministry">` |
| Hero image | Replace `assets/hero.png` |
| Page title / description | `index.html` — `<title>` and `<meta name="description">` |
| Footer links | `index.html` — `<nav class="footer-links">` |
