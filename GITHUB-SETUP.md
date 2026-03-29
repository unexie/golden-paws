# How to Publish Golden Paws to GitHub Pages

Follow these steps once to get your site live. After that, every new blog post just needs to be committed and pushed.

---

## Step 1 — Create a GitHub repository

1. Go to https://github.com/new
2. Name it: `golden-paws` (or anything you like)
3. Set it to **Public**
4. Do NOT check "Add a README" — leave it empty
5. Click **Create repository**

---

## Step 2 — Upload your site files

### Option A — Drag & drop (easiest)
1. Open your new repository on GitHub
2. Click **"uploading an existing file"**
3. Drag the entire `golden-paws-site` folder contents into the window
4. Scroll down, write a commit message like "Initial site launch"
5. Click **Commit changes**

> Important: Upload the FILES inside the folder (index.html, blog.html, posts/ folder), not the folder itself.

### Option B — Git command line
```bash
cd /path/to/golden-paws-site
git init
git add .
git commit -m "Initial site launch"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/golden-paws.git
git push -u origin main
```

---

## Step 3 — Enable GitHub Pages

1. In your repository, go to **Settings** (top menu)
2. Click **Pages** in the left sidebar
3. Under "Branch", select **main** and folder **/ (root)**
4. Click **Save**

Your site will be live within 1–2 minutes at:
**https://YOUR-USERNAME.github.io/golden-paws/**

---

## Step 4 — Adding new blog posts (every week)

When the weekly agent drops a new `.html` file into the `posts/` folder:

1. Go to your GitHub repository
2. Navigate to the `posts/` folder
3. Click **Add file → Upload files**
4. Upload the new post file
5. Also upload the updated `blog.html` (which now has the new post card)
6. Commit — the new post is live instantly!

---

## Optional: Custom domain

If you want a domain like `goldenpaws.com`:
1. Buy a domain from Namecheap, Google Domains, etc.
2. In GitHub Pages settings, enter your custom domain
3. Follow the DNS instructions provided by GitHub

---

## Your site structure

```
golden-paws-site/
├── index.html          ← Homepage
├── blog.html           ← Blog listing page
└── posts/
    ├── new-owner-guide.html      ← First post (live now)
    └── YYYY-MM-DD-[topic].html   ← Added weekly by the agent
```
