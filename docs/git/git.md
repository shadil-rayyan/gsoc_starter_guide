## What is `.git`? (Super simple)

Think of your project folder like a **school notebook**.

* Your code files = the pages
* `.git` = a **hidden history book**

📘 **`.git` stores:**

* every change you ever made
* who made it
* when it was made
* how to go back in time if something breaks

👉 If you delete `.git`, Git forgets everything.
👉 If `.git` exists, the folder is a **Git repository**.

You normally **never touch `.git` manually**. Git commands use it for you.

---

## What is Git? (One sentence)

**Git is a tool that tracks changes in code and helps many people work together safely.**

---

## Why big open-source projects use Git

Big projects have:

* thousands of contributors
* people in different countries
* code changing every minute

Git helps them:

* avoid overwriting each other’s work
* review code before merging
* roll back mistakes instantly

---

# The ONLY Git You Need to Know (for big open source)

We’ll cover **exactly what matters**, nothing extra.

---

## 1️⃣ Create or get a project

### Clone (most common for open source)

```bash
git clone https://github.com/org/project.git
```

📥 This:

* downloads the project
* creates a `.git` folder
* connects your copy to the original project

---

## 2️⃣ Check project status (MOST USED COMMAND)

```bash
git status
```

This tells you:

* what files you changed
* what is ready to save
* what is not saved yet

🧠 Use this **all the time**.

---

## 3️⃣ Save your work (Commit)

Git saves work in **2 steps**.

### Step 1: Select files

```bash
git add file.js
```

or everything:

```bash
git add .
```

### Step 2: Save with a message

```bash
git commit -m "Fix login bug"
```

📦 A **commit** is:

* a snapshot of your code
* with a message explaining why

Big projects care a LOT about good commit messages.

---

## 4️⃣ See history

```bash
git log
```

Shows:

* previous commits
* who made them
* commit messages

Tip:

```bash
git log --oneline
```

---

## 5️⃣ Branches (VERY IMPORTANT)

A **branch** = a safe copy of the code to work on.

Big rule:
❌ Never work directly on `main` / `master`

### Create a branch

```bash
git checkout -b fix-login-bug
```

Now you can:

* break things
* experiment
* work safely

---

## 6️⃣ Switch branches

```bash
git checkout main
```

or newer Git:

```bash
git switch main
```

---

## 7️⃣ Update your code (before working)

```bash
git pull
```

This:

* gets the latest changes
* prevents conflicts

⚠️ Always do this before coding.

---

## 8️⃣ Push your work

```bash
git push origin fix-login-bug
```

This:

* uploads your branch to GitHub
* makes it visible to maintainers

---

## 9️⃣ Pull Requests (How open source really works)

You **never merge yourself** in big projects.

Flow:

1. Fork the repo (GitHub button)
2. Create a branch
3. Commit your changes
4. Push your branch
5. Open a **Pull Request (PR)**

A PR:

* explains what you changed
* lets maintainers review your code
* triggers tests

---

## 🔟 Fix mistakes (important)

### Undo unstaged changes

```bash
git checkout -- file.js
```

### Undo last commit (keep code)

```bash
git reset --soft HEAD~1
```

### Undo last commit (delete code)

```bash
git reset --hard HEAD~1
```

⚠️ Be careful with `--hard`.

---

## 1️⃣1️⃣ Resolve conflicts (will happen)

Conflict = Git doesn’t know which change to keep.

Steps:

1. Open the file
2. Look for:

```text
<<<<<<<
=======
>>>>>>>
```

3. Fix it manually
4. Save file
5. Run:

```bash
git add .
git commit
```

Everyone hits conflicts. Even seniors.

---

## 1️⃣2️⃣ Big open-source rules (VERY IMPORTANT)

✔ Always read `CONTRIBUTING.md`
✔ Follow code style
✔ Small PRs > big PRs
✔ Clear commit messages
✔ Be polite in reviews

---

## Example: Real open-source workflow

```bash
git clone repo
git checkout -b fix-typo
# make changes
git add .
git commit -m "Fix typo in README"
git push origin fix-typo
# open PR on GitHub
```

That’s it.

---

