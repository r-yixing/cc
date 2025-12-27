# 🚀 How to Push Your Decoded Website to GitHub

## Step 1: Create a New Repository on GitHub

1. Go to [github.com](https://github.com) and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Fill in the details:
   - **Repository name**: `decoded-website` (or your preferred name)
   - **Description**: "Decoded landing page - AI-powered skincare analysis app"
   - **Visibility**: Choose Public or Private
   - **DO NOT** initialize with README, .gitignore, or license (we already have these)
5. Click "Create repository"

## Step 2: Push Your Local Repository

After creating your GitHub repository, run these commands in your terminal:

```bash
cd /home/claude/decoded-website

# Add your GitHub repository as remote
git remote add origin https://github.com/YOUR_USERNAME/decoded-website.git

# Push your code to GitHub
git push -u origin main
```

**Replace `YOUR_USERNAME` with your actual GitHub username!**

## Step 3: Enable GitHub Pages (Optional)

To host your website for free on GitHub Pages:

1. Go to your repository on GitHub
2. Click "Settings"
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click "Save"
6. Wait a few minutes, then visit: `https://YOUR_USERNAME.github.io/decoded-website/`

## Alternative: Using GitHub CLI

If you have GitHub CLI installed:

```bash
cd /home/claude/decoded-website

# Create repository and push in one command
gh repo create decoded-website --public --source=. --remote=origin --push
```

## Troubleshooting

### Authentication Issues

If you're using HTTPS and get authentication errors:

1. Use a Personal Access Token instead of password
2. Go to GitHub Settings → Developer settings → Personal access tokens
3. Generate a new token with `repo` scope
4. Use the token as your password when prompted

### Alternative: Using SSH

```bash
# Add SSH remote instead
git remote add origin git@github.com:YOUR_USERNAME/decoded-website.git
git push -u origin main
```

## What's Included in Your Repository

- ✅ `index.html` - Your complete Decoded landing page
- ✅ `README.md` - Comprehensive documentation
- ✅ `LICENSE` - MIT License
- ✅ `CONTRIBUTING.md` - Contribution guidelines
- ✅ `.gitignore` - Files to ignore

## Next Steps

After pushing to GitHub, you can:

1. **Share the repository** with your team
2. **Deploy to GitHub Pages** for free hosting
3. **Set up custom domain** (if you have one)
4. **Enable issues** for bug tracking
5. **Add collaborators** in Settings → Collaborators

## Need Help?

- GitHub Docs: https://docs.github.com
- GitHub Support: https://support.github.com

---

**Happy coding! 💚**
