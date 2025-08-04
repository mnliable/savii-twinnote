# GitHub Repository Setup Commands

## 🚀 Quick Setup

After creating your GitHub repository at https://github.com/new, run these commands:

```bash
# Replace YOUR_USERNAME with your actual GitHub username
git remote add origin https://github.com/YOUR_USERNAME/savii-nova-epk.git
git branch -M main
git push -u origin main
```

## 📋 Repository Creation Steps

1. **Go to GitHub**: https://github.com/new
2. **Repository name**: `savii-nova-epk`
3. **Visibility**: Public (required for GitHub Pages)
4. **DO NOT** check "Add a README file"
5. **DO NOT** check "Add .gitignore"
6. **DO NOT** check "Choose a license"
7. **Click**: "Create repository"

## 🌐 Enable GitHub Pages

After pushing your code:

1. Go to your repository on GitHub
2. Click **Settings** tab
3. Scroll down to **Pages** section
4. Under **Source**, select **Deploy from a branch**
5. Select **main** branch and **/ (root)** folder
6. Click **Save**

## 🎉 Your EPK will be live at:
`https://YOUR_USERNAME.github.io/savii-nova-epk`

## 📁 What's Being Pushed

- ✅ `build/index.html` - Main EPK page
- ✅ `build/Press photos/` - All press photos
- ✅ `build/songs/` - All audio files
- ✅ `build/README.md` - Documentation
- ✅ `build/DEPLOYMENT_CHECKLIST.md` - Launch checklist
- ✅ `.gitignore` - Excludes development files

## 🔄 Future Updates

To update your EPK:

```bash
git add build/
git commit -m "Update EPK content"
git push origin main
```

GitHub Pages will automatically deploy your changes! 