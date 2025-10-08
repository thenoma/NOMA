# 🚀 Deploying NOMA to GitHub Pages

Your NOMA website is ready to deploy! Follow these simple steps:

## ✅ Step 1: Local Setup (Completed)
- ✓ Git repository initialized
- ✓ Files committed to `main` branch
- ✓ Ready to push to GitHub

## 📦 Step 2: Create GitHub Repository

### Option A: Using GitHub Website (Easiest)

1. **Go to GitHub**: Visit [github.com](https://github.com) and log in

2. **Create New Repository**:
   - Click the `+` icon in the top right → "New repository"
   - Repository name: `NOMA` (or `noma-website`)
   - Description: "Network of Moroccans in America - Official Website"
   - Make it **Public** (required for free GitHub Pages)
   - **DO NOT** initialize with README, .gitignore, or license (we already have these)
   - Click "Create repository"

3. **Copy the repository URL** (it will look like):
   ```
   https://github.com/YOUR-USERNAME/NOMA.git
   ```

4. **Push your code** - Open Terminal and run:
   ```bash
   cd /Users/mt/Workspace/NOMA
   git remote add origin https://github.com/YOUR-USERNAME/NOMA.git
   git push -u origin main
   ```

### Option B: Using GitHub CLI (If you prefer command line)

1. **Install GitHub CLI**:
   ```bash
   brew install gh
   ```

2. **Authenticate**:
   ```bash
   gh auth login
   ```

3. **Create repository and push**:
   ```bash
   cd /Users/mt/Workspace/NOMA
   gh repo create NOMA --public --source=. --remote=origin --push
   ```

## 🌐 Step 3: Enable GitHub Pages

1. **Go to your repository** on GitHub
   - Navigate to: `https://github.com/YOUR-USERNAME/NOMA`

2. **Go to Settings**:
   - Click the "Settings" tab (⚙️ icon)

3. **Enable Pages**:
   - Scroll down to "Pages" in the left sidebar
   - Under "Source", select: **Branch: main** and **Folder: / (root)**
   - Click "Save"

4. **Wait for deployment** (1-2 minutes)
   - GitHub will show: "Your site is ready to be published at..."
   - The URL will be: `https://YOUR-USERNAME.github.io/NOMA/`

5. **Visit your live website!** 🎉

## 🔄 Making Updates

After your initial deployment, any time you want to update the website:

```bash
cd /Users/mt/Workspace/NOMA

# Make your changes to index.html, styles.css, or script.js

# Commit and push
git add .
git commit -m "Description of your changes"
git push
```

GitHub Pages will automatically redeploy within 1-2 minutes!

## 🎨 Custom Domain (Optional)

Want to use a custom domain like `www.nomausa.org`?

1. **Buy a domain** from providers like Namecheap, GoDaddy, or Google Domains

2. **Configure DNS**:
   - Add a CNAME record pointing to: `YOUR-USERNAME.github.io`
   - Or for apex domain, add A records:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153

3. **In GitHub Settings → Pages**:
   - Enter your custom domain in the "Custom domain" field
   - Enable "Enforce HTTPS" (wait 24 hours for SSL certificate)

## 📊 Monitoring

- **Check deployment status**: Visit your repository → "Actions" tab
- **View analytics**: GitHub Pages doesn't include analytics, but you can add:
  - Google Analytics
  - Plausible Analytics
  - Simple Analytics

## 🆘 Troubleshooting

**Site not showing up?**
- Make sure the repository is public
- Check that GitHub Pages is enabled with source set to `main` branch
- Wait 2-3 minutes for initial deployment
- Clear your browser cache

**404 Error?**
- Verify the file is named `index.html` (lowercase)
- Check the branch is `main` in GitHub Pages settings

**Contact form not working?**
- Currently shows an alert - to make it functional:
  - Use [Formspree](https://formspree.io) (free tier available)
  - Use [EmailJS](https://www.emailjs.com) (free tier available)
  - Or integrate with a backend service

## 📝 Quick Reference

**Your Local Path**: `/Users/mt/Workspace/NOMA`

**Repository URL**: `https://github.com/YOUR-USERNAME/NOMA`

**Live Website**: `https://YOUR-USERNAME.github.io/NOMA/`

---

Need help? Check GitHub's [Pages documentation](https://docs.github.com/en/pages) or contact support!

