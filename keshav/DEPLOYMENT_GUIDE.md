# Netlify Deployment Guide

## Quick Deployment Steps

### Method 1: Drag and Drop (5 minutes)

1. **Go to Netlify**: Visit [netlify.com](https://netlify.com)
2. **Sign Up**: Create a free account (GitHub login recommended)
3. **Deploy Site**: 
   - Look for "Want to deploy a new site without connecting to Git?"
   - Select all project files from `c:\Users\pbsns\Downloads\keshav`
   - Drag files to the deployment area
4. **Get Live URL**: Copy your instant live URL (e.g., `https://wonderful-einstein-123456.netlify.app`)

### Method 2: GitHub Integration (10 minutes)

1. **Create GitHub Repository**:
   ```bash
   # On GitHub, create new repository: bootstrap5-modern-website
   git remote add origin https://github.com/YOUR_USERNAME/bootstrap5-modern-website.git
   git branch -M main
   git push -u origin main
   ```

2. **Connect Netlify**:
   - Netlify Dashboard → "New site from Git"
   - Choose "GitHub" → Select your repository
   - Build settings: Leave empty (static HTML site)
   - Click "Deploy site"

## Post-Deployment

### Update README with Live URL
Once deployed, update the README.md file:
```markdown
## 🚀 Live Demo
[View Live Website](YOUR_NETLIFY_URL_HERE)
```

### Custom Domain (Optional)
- Netlify Dashboard → Site settings → Domain management
- Add custom domain if you have one

### Form Handling Enhancement
Your contact form can use Netlify's built-in form handling:
```html
<!-- Add to your form tag in contact.html -->
<form netlify>
```

## Files to Deploy
✅ index.html - Home page
✅ about.html - About page  
✅ contact.html - Contact page
✅ README.md - Documentation
✅ PROJECT_REFLECTION.md - Project report

## Expected Result
- Live website accessible via HTTPS
- Automatic SSL certificate
- Global CDN for fast loading
- Mobile-responsive across all devices

## Troubleshooting
- **404 errors**: Ensure index.html is in root directory
- **CSS not loading**: Check Bootstrap CDN links
- **Form not working**: Add `netlify` attribute to form tag

Your Bootstrap 5 website will be live in under 2 minutes with drag-and-drop deployment!