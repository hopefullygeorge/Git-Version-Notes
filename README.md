# **Git Version Control – Quick Guide** 🚀  

## **1️⃣ Understanding the Workflow**  
📂 **Working Directory** → 📌 **Staging Area** → ✅ **Commit (Local Repository)** → 🌍 **Push to Remote Repository (GitHub)**  

---

## **2️⃣ Essential Git Commands**  

### **🛠 Initial Setup**  
- `git init` → Initialize an empty Git repository in a folder.  
- `git status` → Check the status of your working directory and staging area.  

### **📌 Staging & Unstaging**  
- `git add file_name` → Add a specific file to the staging area.  
- `git add .` → Add **all untracked files** to the staging area.  
- `git rm --cached -r .` → Remove everything from the staging area (but keep the files locally).  

### **✅ Committing Changes**  
- `git commit -m "Commit message here"` → Commit staged changes with a meaningful message _(written in present tense, e.g., "Complete Chapter 1")_.  
- `git log` → View commit history.  

### **📊 Viewing Changes**  
- `git diff file_name_here` → Show differences between the **last commit** and **current changes**.  
- `git checkout file_name_here` → Revert a file back to the last committed version.  

---

## **3️⃣ Branching & Merging**  
- `git branch name_of_branch` → Create a new branch.  
- `git branch` → List all branches (`*` indicates the currently selected branch).  
- `git checkout name_of_branch` → Switch to a different branch.  
- `git merge branch_name` → Merge a specified branch into the current branch.  

---

## **4️⃣ Connecting to GitHub**  

### **🔗 Setting Up a Remote Repository**  
1️⃣ Create a remote repository on GitHub.  
2️⃣ Connect it to your local repo:  
   ```sh
   git remote add origin <url_of_remote_repository>
   ```
   _(`origin` is the default name for the remote repository, but you can change it.)_  

3️⃣ Push your local repository to GitHub:  
   ```sh
   git push -u origin master
   ```
   _(`-u` links the local branch with the remote branch for future pushes.)_  

### **📥 Cloning a Remote Repository**  
- `git clone <url_of_repository>` → Clone an existing repository to your local machine.  

---

## **5️⃣ Handling Ignored Files**  
- Create a `.gitignore` file to specify which files **should not be tracked**.  
- Inside `.gitignore`:  
  ```sh
  *.txt  # Ignore all text files
  /node_modules/  # Ignore a specific directory
  secrets.env  # Ignore a specific file
  ```

---

### **🚀 Pro Tip:**  
Use **meaningful commit messages** and **branch names** to keep your Git history clear and readable!  
