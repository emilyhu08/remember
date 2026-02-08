# GitHub Pages Setup Instructions

## What I Created

Your GitHub Pages site is ready! Here's what's included:

```
github-pages-site/
├── index.html                    # Homepage with all your apps
└── remember/
    ├── privacy.html             # Privacy Policy for Remember app
    └── support.html             # Support page with FAQ
```

## URLs After Deployment

Once deployed to `emilyhu08.github.io`, your URLs will be:

- **Homepage:** `https://emilyhu08.github.io`
- **Privacy Policy:** `https://emilyhu08.github.io/remember/privacy.html`
- **Support:** `https://emilyhu08.github.io/remember/support.html`

## How to Deploy

### Step 1: Create the GitHub Repository

1. Go to https://github.com/new
2. **Repository name:** `emilyhu08.github.io` (must be exactly this)
3. **Description:** "Zhiying Hu - Personal website and app support pages"
4. **Public** (must be public for GitHub Pages)
5. Click "Create repository"

### Step 2: Push Your Files

```bash
cd /Users/emily/Repos/remember-app/github-pages-site

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: Add homepage and Remember app pages"

# Add remote (replace with your actual repo URL)
git remote add origin https://github.com/emilyhu08/emilyhu08.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (in left sidebar)
3. Under "Source", select:
   - Branch: **main**
   - Folder: **/ (root)**
4. Click **Save**
5. Wait 1-2 minutes for deployment

### Step 4: Verify

Visit `https://emilyhu08.github.io` - your site should be live!

## Use in App Store Connect

Now you can use these URLs in your App Store submission:

- **Privacy URL:** `https://emilyhu08.github.io/remember/privacy.html`
- **Support URL:** `https://emilyhu08.github.io/remember/support.html`

## Adding More Apps Later

When you create a new app, just:

1. Add a new card to `index.html` in the apps grid
2. Create a new folder (e.g., `myapp/`)
3. Copy `privacy.html` and `support.html` from `remember/`
4. Update the content for your new app
5. Push to GitHub

## Customization

Feel free to customize:

- **Colors:** Update the CSS gradient in `index.html` (currently green to match your app)
- **Email:** I used `emilyhu08@gmail.com` - update if you want a different contact email
- **Content:** All content is editable in the HTML files

## Preview Locally (Optional)

To preview before deploying:

```bash
cd /Users/emily/Repos/remember-app/github-pages-site
python3 -m http.server 8000
```

Then visit: `http://localhost:8000`

---

Your GitHub Pages site is ready to deploy! 🚀
