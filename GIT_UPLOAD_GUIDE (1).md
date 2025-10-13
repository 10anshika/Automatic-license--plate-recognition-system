# 🚀 Complete Guide: Uploading Your ANPR Project to GitHub

## Step 1: Find Your Project Folder Path

### Method 1: Using Windows Explorer (Easiest)
1. Open File Explorer and navigate to your ANPR project folder
2. Right-click inside the folder and select **"Git Bash Here"**
3. Skip to Step 3 (no path needed!)

### Method 2: Find Path Manually
1. Navigate to your project folder in Windows Explorer
2. Click on the address bar at the top
3. Copy the full path (e.g., `C:\Users\YourName\Documents\ANPR Project`)

## Step 2: Open Git Bash

### Option A: Right-click Method (Recommended)
- Right-click in your project folder → Select "Git Bash Here"

### Option B: Start Menu Method
- Press Windows key → Type "Git Bash" → Press Enter
- Navigate to your project: `cd /c/Users/YourName/Documents/ANPR\ Project`

## Step 3: Initialize Git Repository

```bash
# Check current location
pwd

# Initialize Git repository
git init

# Check Git status
git status
```

## Step 4: Add Files to Git

```bash
# Add all files
git add .

# Or add specific files
git add ANPR_PROJECT.ipynb
git add requirements.txt
git add README.md
git add "Automatic-License-Plate-Recognition-System.pptx"

# Check what's been added
git status
```

## Step 5: Make Initial Commit

```bash
# Commit with descriptive message
git commit -m "Initial commit: ANPR project with Jupyter notebook and presentation"

# Verify commit
git log --oneline
```

## Step 6: Connect to GitHub Repository

```bash
# Add remote repository (use your actual GitHub URL)
git remote add origin https://github.com/10anshika/Automatic-license--plate-recognition-system.git

# Verify remote
git remote -v

# Set main branch
git branch -M main
```

## Step 7: Push to GitHub

```bash
# Push files to GitHub
git push -u origin main
```

## 🔧 Common Issues & Solutions

### Issue 1: "Git command not found"
**Solution**: Install Git from https://git-scm.com/downloads

### Issue 2: "Permission denied"
**Solution**: Configure Git credentials:
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@gmail.com"
```

### Issue 3: "Repository already exists"
**Solution**: 
```bash
git pull origin main --allow-unrelated-histories
git push -u origin main
```

### Issue 4: Large files error
**Solution**: Use quotes for files with spaces:
```bash
git add "Automatic-License-Plate-Recognition-System.pptx"
```

## 📋 Complete Command Sequence (Copy & Paste)

```bash
# Navigate to project (if needed)
cd /path/to/your/project

# Initialize and add files
git init
git add .
git status

# Commit changes
git commit -m "Initial commit: ANPR project with Jupyter notebook and presentation"

# Connect to GitHub
git remote add origin https://github.com/10anshika/Automatic-license--plate-recognition-system.git
git branch -M main

# Push to GitHub
git push -u origin main
```

## 🎉 Verification

After successful upload, check:
1. Go to your GitHub repository
2. Verify all files are present:
   - ✅ ANPR_PROJECT.ipynb
   - ✅ requirements.txt
   - ✅ README.md
   - ✅ Automatic-License-Plate-Recognition-System.pptx

## 📝 Future Updates

For future changes:
```bash
# Make changes to your files
# Then add, commit, and push:

git add .
git commit -m "Description of changes"
git push origin main
```

## 🚨 Important Notes

- Always commit before pushing
- Use descriptive commit messages
- Check git status frequently
- Keep sensitive data out of public repos
- Test your notebook runs before committing

---

**Need help?** Create an issue in your GitHub repository or check the Git documentation.
