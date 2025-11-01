# 🚀 Git and GitHub Commands Essentials for Beginners 💡

Welcome! This is a quick visual guide to the most important basic Git commands, designed to **simplify your understanding** of the Git workflow and how to interact with GitHub.

---

## 1. 🔄 The Git Workflow: Local and Remote

![Git Workflow: Workspace, Stage, Local, Remote](pics/pic01.jpg)

This image illustrates the core stages of the Git workflow and how changes move through them, up to the **Remote Repository**.

### Stages and Key Commands Explained:

| Stage | Description | Key Commands |
| :--- | :--- | :--- |
| **Workspace (Working Directory)** | Where you write and modify your files on your local machine. | `git restore <file>`: Discards changes in a file, reverting to its last Staged or Committed state. |
| **Stage (Index)** | A temporary area where you select and gather changes you want to include in your next **Commit**. | `git add <file>` or `git add .`: Adds modified files from the **Workspace** to the **Stage**. |
| **Local Repository** | A database on your machine that stores all your **Commits** and the complete history of your project. | `git commit -m "Message"`: Permanently saves the staged changes into the **Local Repository**. |
| **Remote Repository** | A copy of your project hosted online (e.g., **GitHub** or **GitLab**) for collaboration and backup. | `git push`: Sends your local **Commits** to the Remote Repository.<br>`git fetch`: Downloads new changes from the Remote Repository *without* integrating them.<br>`git pull`: Fetches and merges new changes from the Remote Repository. |

---

## 2. ⬆️ Pushing a New Project to GitHub

![Git Steps: Initialize and Push First Project](pics/pic03.jpg)

These steps guide you on how to **initialize** your local project and connect it to a new repository on GitHub for the **first time**.

### Step-by-Step Commands:

1. `echo "#Project" > README.md` – *(Optional)* Creates a basic `README.md` file.  
2. `git init` – **Initializes** your project folder as a local Git repository.  
3. `git add .` – **Stages** all current project files for the next commit.  
4. `git commit -m "Edit1"` – **Commits** the staged changes as the first save point.  
5. `git remote add origin <GitHub Link>` – **Connects** your local repository to the remote one on GitHub.  
6. `git branch -M main` – **Renames** the current branch to `main`.  
7. `git push origin main` – **Uploads** all local commits to the remote repository (`origin`).  

---

## 3. ⬇️ Cloning, Updating, and Modifying from GitHub

![Git Steps: Clone, Update, and Push Changes](pics/pic02.jpg)

This section provides the workflow for **cloning** an existing project, making modifications, and keeping your local and remote branches synchronized.

### Workflow Steps:

#### 1️⃣ Clone the Project (First Time)

```bash
cd <folder>
git clone <GitHub Link>
