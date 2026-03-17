# IPMAT Planner

Personal study planner for IPMAT 2025 prep.

## Deploy to Vercel

### Option A — Vercel CLI (fastest)

```bash
# 1. Install Vercel CLI (only once)
npm install -g vercel

# 2. Go into the project folder
cd ipmat-planner

# 3. Deploy
vercel

# Follow the prompts:
#   Set up and deploy? → Y
#   Which scope? → your account
#   Link to existing project? → N
#   Project name? → ipmat-planner (or anything)
#   In which directory is your code? → ./public
#   Want to modify settings? → N

# Done — you'll get a live URL like: https://ipmat-planner.vercel.app
```

### Option B — GitHub + Vercel Dashboard

```bash
# 1. Create a GitHub repo and push this folder
git init
git add .
git commit -m "init"
git remote add origin https://github.com/YOUR_USERNAME/ipmat-planner.git
git push -u origin main
```

Then go to vercel.com → New Project → Import your GitHub repo → set **Root Directory** to `public` → Deploy.

## Project Structure

```
ipmat-planner/
├── public/
│   ├── index.html   ← entire app (single file)
│   ├── logo.svg     ← axis mark, light variant
│   └── favicon.svg  ← dark background favicon
├── vercel.json      ← routing config
└── README.md
```

## Notes

- All data is saved in **localStorage** — works offline, persists on the same browser/device
- No backend, no dependencies, no build step needed
- To update: edit `public/index.html` and push to GitHub (auto-deploys via Vercel)
