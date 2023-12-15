# GitHub Cheatsheet

## 1. **Initialize a Repository**

### Create a New Repository
```bash
git init
```

### Clone a Repository
```bash
git clone repository_url
```

## 2. **Make Changes**

### Check Status
```bash
git status
```

### Add Changes to Staging
```bash
git add .
```

### Commit Changes
```bash
git commit -m "Commit message"
```

## 3. **Branching**

### Create a New Branch
```bash
git branch branch_name
```

### Switch to a Branch
```bash
git checkout branch_name
```

### Create and Switch to a New Branch
```bash
git checkout -b new_branch_name
```

## 4. **Merge and Pull**

### Merge Changes
```bash
git merge branch_name
```

### Pull Changes from a Remote Repository
```bash
git pull origin branch_name
```

## 5. **Push Changes to a Remote Repository**

### Push Changes to the Current Branch
```bash
git push origin branch_name
```

### Push Changes to a Different Branch
```bash
git push origin local_branch_name:remote_branch_name
```

## 6. **Pull Requests**

### Create a Pull Request
```bash
git request-pull branch_name repository_url
```

## 7. **View Changes**

### View Changes Made
```bash
git log
```

### View Remote Repositories
```bash
git remote -v
```

## 8. **Undo Changes**

### Undo the Last Commit
```bash
git reset HEAD~
```

### Discard Changes in Working Directory
```bash
git checkout -- .
```

## 9. **Gitignore**

### Create a Gitignore File
```bash
touch .gitignore
```

### Add Files to Gitignore
```bash
echo "file_name" >> .gitignore
```

## 10. **GitHub Actions**

### Create a GitHub Actions Workflow
```bash
mkdir .github/workflows
touch .github/workflows/workflow.yml
```

## 11. **Git Tags**

### Create a Tag
```bash
git tag tag_name
```

### Push Tags to Remote Repository
```bash
git push origin tag_name
```

## 12. **Git Config**

### Set User Configurations
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

## 13. **Miscellaneous**

### Show the Git Help
```bash
git --help
```
