# GitHub Repository Setup & Deployment Guide

## Step 1: Create GitHub Repository

1. **Go to GitHub**: Visit [github.com](https://github.com) and log into your account
2. **Create New Repository**: 
   - Click the "+" icon in the top right → "New repository"
   - Repository name: `responsive-bootstrap-website`
   - Description: "Modern responsive website built with Bootstrap 5 - Internship Project"
   - Make it **Public** (required for free GitHub Pages)
   - **DO NOT** initialize with README (we already have files)
   - Click "Create repository"

## Step 2: Connect Local Project to GitHub

Run these commands in your terminal from the project directory:

```bash
# Add the GitHub repository as remote origin
git remote add origin https://github.com/YOUR_USERNAME/responsive-bootstrap-website.git

# Rename the default branch to 'main'
git branch -M main

# Push all files to GitHub
git push -u origin main
```

**Replace `YOUR_USERNAME` with your actual GitHub username!**

## Step 3: Verify Upload

Check your GitHub repository page - you should see:
- ✅ index.html
- ✅ about.html  
- ✅ contact.html
- ✅ README.md
- ✅ PROJECT_REFLECTION.md
- ✅ DEPLOYMENT_GUIDE.md

## Step 4: Deploy to Netlify

### Option A: GitHub Integration (Recommended)
1. Go to [netlify.com](https://netlify.com) → Login/Sign up
2. Click "New site from Git"
3. Choose "GitHub" → Authorize Netlify
4. Select "responsive-bootstrap-website" repository
5. Deploy settings:
   - Build command: (leave empty)
   - Publish directory: (leave empty)
6. Click "Deploy site"

### Option B: Direct Deployment
1. Go to [netlify.com](https://netlify.com) → Login/Sign up
2. Drag and drop all project files to deployment area
3. Get instant live URL

## Step 5: Enable GitHub Pages (Bonus)

1. Go to your GitHub repository
2. Settings → Pages (in sidebar)
3. Source: Deploy from a branch
4. Branch: main → / (root) → Save
5. Your site will be available at: `https://YOUR_USERNAME.github.io/responsive-bootstrap-website`

## Final Deliverables

Once completed, you'll have:

**GitHub Repository URL**: `https://github.com/YOUR_USERNAME/responsive-bootstrap-website`  
**Netlify Live URL**: `https://wonderful-name-12345.netlify.app` (example)  
**GitHub Pages URL**: `https://YOUR_USERNAME.github.io/responsive-bootstrap-website`

## Update README with Live URLs

After deployment, update your README.md:

```markdown
## 🚀 Live Demo
[View on Netlify](YOUR_NETLIFY_URL)  
[View on GitHub Pages](YOUR_GITHUB_PAGES_URL)

## 📁 Repository
[GitHub Repository](https://github.com/YOUR_USERNAME/responsive-bootstrap-website)
```

## Commands Summary

```bash
# Connect to GitHub
git remote add origin https://github.com/YOUR_USERNAME/responsive-bootstrap-website.git
git branch -M main
git push -u origin main

# For future updates
git add .
git commit -m "Update message"
git push
```

Your Bootstrap 5 website will be live on both Netlify and GitHub Pages!