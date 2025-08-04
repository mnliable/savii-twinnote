# Custom Domain Troubleshooting Guide

## 🔍 Current Status

✅ **DNS Configuration**: Correctly pointing to GitHub Pages servers
✅ **Repository Structure**: Files moved to root directory
✅ **CNAME File**: Added to repository
✅ **Git Push**: Successfully pushed to GitHub

## ❌ Issue: Domain returning 404

The domain `savii-twinnote.ca` is returning a 404 error, which indicates GitHub Pages is not properly enabled.

## 🛠️ Troubleshooting Steps

### 1. Enable GitHub Pages

**Go to**: https://github.com/mnliable/savii-twinnote/settings/pages

**Configure**:
- Source: **Deploy from a branch**
- Branch: **main**
- Folder: **/ (root)**
- Click **Save**

### 2. Verify Custom Domain

**In GitHub Pages settings**:
- Custom domain: `savii-twinnote.ca`
- Check "Enforce HTTPS" (recommended)
- Click **Save**

### 3. Check Repository Structure

The repository should now have:
```
savii-twinnote/
├── index.html          ✅ (main EPK page)
├── CNAME              ✅ (custom domain)
├── Press photos/      ✅ (press photos)
├── songs/             ✅ (audio files)
├── README.md          ✅ (documentation)
└── .gitignore         ✅ (excludes dev files)
```

### 4. DNS Verification

The domain should resolve to GitHub Pages IPs:
- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

✅ **Status**: DNS is correctly configured

### 5. Wait for Deployment

GitHub Pages can take up to 10 minutes to deploy after changes.

### 6. Test URLs

Try these URLs to verify:
- https://mnliable.github.io/savii-twinnote
- http://savii-twinnote.ca
- https://savii-twinnote.ca

## 🚨 Common Issues

### Issue 1: GitHub Pages Not Enabled
**Solution**: Enable in repository Settings → Pages

### Issue 2: Wrong Branch/Folder
**Solution**: Ensure deploying from `main` branch and `/ (root)` folder

### Issue 3: Custom Domain Not Configured
**Solution**: Add domain in Pages settings and ensure CNAME file exists

### Issue 4: SSL Certificate Issues
**Solution**: Wait for GitHub to provision SSL certificate (can take up to 24 hours)

## 📞 Next Steps

1. **Enable GitHub Pages** in repository settings
2. **Configure custom domain** in Pages settings
3. **Wait 10-15 minutes** for deployment
4. **Test the domain** again

## 🔗 Useful Links

- Repository: https://github.com/mnliable/savii-twinnote
- Pages Settings: https://github.com/mnliable/savii-twinnote/settings/pages
- GitHub Pages Docs: https://docs.github.com/en/pages 