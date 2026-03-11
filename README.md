# Bitcoin Price & Ukraine Aid — Data Visualization

An interactive dual-axis chart comparing Bitcoin's price history with international aid to Ukraine (2010–2026), with annotated peak events.

**Live demo:** `https://<your-username>.github.io/<your-repo-name>/`
https://Vitaliitymashkov.github.io/bitcoin-ua/
---

## 🚀 Deploy to GitHub Pages (step by step)

### 1. Create a new GitHub repository

Go to [github.com/new](https://github.com/new) and create a repository.  
Name it anything — e.g. `btc-ukraine-viz`.  
Set it to **Public** (required for free GitHub Pages).

### 2. Push this project

```bash
cd btc-ukraine-viz

git init
git add .
git commit -m "Initial commit"

git remote add origin https://github.com/<your-username>/<your-repo-name>.git
git branch -M main
git push -u origin main
```

### 3. Enable GitHub Pages with GitHub Actions

1. Go to your repo on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under **Source**, select **GitHub Actions**
4. That's it — no further config needed

### 4. Trigger the deployment

The workflow runs automatically on every push to `main`.  
You can also trigger it manually:

1. Go to **Actions** tab in your repo
2. Click **Deploy to GitHub Pages**
3. Click **Run workflow** → **Run workflow**

### 5. Visit your site

After ~30 seconds the action completes.  
Your site will be live at:

```
https://<your-username>.github.io/<your-repo-name>/
```

The URL is also shown in the **Actions** run summary and in **Settings → Pages**.

---

## 📁 Project structure

```
.
├── index.html                  # The visualization (self-contained)
└── .github/
    └── workflows/
        └── deploy.yml          # GitHub Actions pipeline
```

---

## 🔄 Updating the site

Just push any change to `main` — the pipeline redeploys automatically:

```bash
git add index.html
git commit -m "Update chart data"
git push
```

---

## 📊 Data sources

| Dataset | Source |
|---|---|
| Bitcoin price | CoinMarketCap, Coinbase historical |
| Ukraine aid | Kiel Institute Ukraine Support Tracker, IMF, EU Commission, World Bank |

Values are approximate year-end figures. 2025–2026 are partial/projected.
