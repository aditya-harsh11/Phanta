# Manual Push Instructions

## Step 1: Create the GitHub Repository

1. Go to https://github.com/new
2. Repository name: `Phanta`
3. Owner: `Aditya Harshavardhan`
4. Description: `AI-Powered Crypto Banking Assistant for Solana`
5. Choose Public or Private
6. **DO NOT** initialize with README, .gitignore, or license (we have these)
7. Click "Create repository"

## Step 2: Push Your Code

After creating the repo, GitHub will show you commands. Use these:

```bash
cd /Users/aditya/Documents/Phanta

# Add your new remote (replace with your actual repo URL)
git remote add origin https://github.com/YOUR_GITHUB_USERNAME/Phanta.git

# Push to GitHub
git push -u origin main
```

## Alternative: Using GitHub CLI

If you have GitHub CLI installed and authenticated:

```bash
cd /Users/aditya/Documents/Phanta
gh repo create YOUR_GITHUB_USERNAME/Phanta --public --source=. --remote=origin --push
```

## Verification

After pushing, verify:
- All files are present
- Repository is under your account

