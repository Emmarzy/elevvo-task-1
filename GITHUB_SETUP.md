# GitHub Setup Guide

## Step-by-Step: Connect Your Repository to GitHub

### 1. Create a New Repository on GitHub
- Go to https://github.com/new
- Repository name: `elevvo-ml-internship` (or your preferred name)
- Description: "Solutions to Elevvo Machine Learning Internship Tasks"
- Choose: **Public** (to showcase your work) or **Private** (if preferred)
- **DO NOT** initialize with README (we already have one)
- Click "Create repository"

### 2. Add Remote and Push
After creating the repository, GitHub will show you these commands. Replace `USERNAME` with your GitHub username:

```bash
# Add the remote (copy the URL from GitHub)
git remote add origin https://github.com/USERNAME/elevvo-ml-internship.git

# Rename main branch if needed
git branch -M main

# Push your initial commit
git push -u origin main
```

### 3. Verify Connection
```bash
git remote -v
```

You should see:
```
origin  https://github.com/USERNAME/elevvo-ml-internship.git (fetch)
origin  https://github.com/USERNAME/elevvo-ml-internship.git (push)
```

---

## Workflow for Each Task

### After Completing Each Task:

```bash
# 1. Check status
git status

# 2. Stage your changes
git add Elevvo\ Internship\ Tasks/task_solution.ipynb

# 3. Commit with descriptive message
git commit -m "Completed Task [N]: [Task Description]

- Summary of what was done
- Key findings or results
- Any challenges overcome"

# 4. Push to GitHub
git push origin main
```

### Example Commit Messages:

```
Completed Task 1: Data Loading and Exploration

- Loaded and explored the dataset
- Performed initial data analysis
- Identified missing values and data types
- Visualized feature distributions
```

```
Completed Task 2: Model Training and Evaluation

- Split data into train/test sets (80/20)
- Trained multiple ML models
- Achieved 92% accuracy with Random Forest
- Generated evaluation metrics and visualizations
```

---

## Useful Git Commands

```bash
# View commit history
git log --oneline

# See changes since last commit
git diff

# Undo last commit (keep changes)
git reset --soft HEAD~1

# View remote branches
git branch -a

# Pull latest changes (if working on multiple machines)
git pull origin main
```

---

## Tips for Success

✅ **Do:**
- Commit after completing each task
- Use clear, descriptive commit messages
- Push daily to avoid losing work
- Document your approach in notebooks

❌ **Don't:**
- Forget to push your changes
- Use vague commit messages like "work" or "fix"
- Store large files (use `.gitignore`)
- Commit sensitive data (API keys, passwords)

---

For more help, visit: https://docs.github.com/en/get-started
