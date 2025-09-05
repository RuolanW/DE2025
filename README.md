# DE2025
The lab materials for the data engineering course at JADS : 2025/2026 edition.

## 🚀 Git Workflow Guide (Safe for Fork)

This section explains how to work safely in **your own fork** (`origin`) without ever affecting the teacher’s repository (`upstream`).

---

### 🌟 Remotes
- **origin** → your fork (e.g., `https://github.com/RuolanW/DE2025.git`)  
- **upstream** → teacher’s repo (e.g., `https://github.com/IndikaKuma/DE2025.git`)  

Check with:
```bash
git remote -v

# Create a new branch for development
git checkout -b feature/mywork

# Stage and commit changes
git add .
git commit -m "feat: my changes"

# Push branch to your fork
git push origin feature/mywork

# Switch to main branch
git checkout main

# Merge your feature branch
git merge feature/mywork

# Push to your fork
git push origin main

# Fetch latest changes from teacher
git fetch upstream

# Merge them into your main branch
git checkout main
git merge upstream/main

# Push the updated main to your fork
git push origin main

