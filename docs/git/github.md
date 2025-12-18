

# GitHub Terms & Features (Big Open Source Survival Guide)

---

## 1️⃣ Repository (Repo)

A **repository** is the project.

It contains:

* code
* issues
* pull requests
* documentation
* history

📦 Think: **one repo = one project**

---

## 2️⃣ Fork (VERY IMPORTANT)

A **fork** is **your own copy** of someone else’s repo.

Why forks exist:

* you don’t have permission to push to the main repo
* you work safely in your own copy

Flow:

```
Original Repo → Fork → Your Changes → Pull Request
```

---

## 3️⃣ Clone

Download a repo (or your fork) to your computer.

```bash
git clone https://github.com/yourname/project.git
```

---

## 4️⃣ Upstream

**Upstream** = the original repo (not your fork)

Used to stay updated.

```bash
git remote add upstream https://github.com/org/project.git
git pull upstream main
```

---

## 5️⃣ Branch

A **branch** is a separate line of work.

Big projects require:

* one branch per feature or fix
* no direct commits to `main`

Example:

```bash
fix-login-bug
docs-update
feature-auth
```

---

## 6️⃣ Pull Request (PR) 🚀

A **Pull Request** is:

> “Please review and merge my changes.”

PR includes:

* code changes
* explanation
* discussion
* tests results

Big open source lives on PRs.

---

## 7️⃣ Review

Maintainers or contributors:

* read your code
* leave comments
* request changes
* approve or reject

### Common review terms:

* **LGTM** → Looks Good To Me
* **Requested Changes** → fix things
* **Approve** → ready to merge

---

## 8️⃣ Merge

**Merge** = combine your PR into the main project.

Usually done by:

* maintainers
* bots (after approval)

You rarely merge your own PR in big projects.

---

## 9️⃣ Issue 🐞

An **Issue** is a tracked problem or task.

Used for:

* bugs
* feature requests
* discussions
* questions

---

## 🔟 Issue Labels

Labels help organize issues.

Common labels:

* `good first issue` (beginner friendly)
* `help wanted`
* `bug`
* `enhancement`
* `discussion`
* `blocked`

👉 **Start with `good first issue`**

---

## 1️⃣1️⃣ Issue Assignment

Someone is responsible for the issue.

* Assigned → someone is working on it
* Unassigned → available

Always **comment before starting work**:

> “Can I work on this?”

---

## 1️⃣2️⃣ Milestone

A **milestone** = group of issues for a release.

Example:

```
v2.0
Bugfix Sprint
Security Patch
```

---

## 1️⃣3️⃣ README.md

The **front page** of the project.

Contains:

* what the project does
* how to run it
* how to contribute

Always read this first.

---

## 1️⃣4️⃣ CONTRIBUTING.md (CRITICAL)

This file tells you:

* how to submit PRs
* naming rules
* branch rules
* commit message style
* testing rules

❌ Ignoring this = PR rejected

---

## 1️⃣5️⃣ CODE_OF_CONDUCT.md

Rules for behavior.

Used to:

* prevent harassment
* enforce respectful communication

Violations can get you banned.

---

## 1️⃣6️⃣ LICENSE 📜

Defines **legal rights**.

Common licenses:

* MIT → very free
* Apache 2.0 → free + patent protection
* GPL → must share changes

Never ignore license rules.

---

## 1️⃣7️⃣ Discussions

Used for:

* ideas
* design talks
* long conversations

Better than opening issues for questions.

---

## 1️⃣8️⃣ Projects (GitHub Projects)

A **board** to track work.

Columns:

* To Do
* In Progress
* Review
* Done

Used in large orgs.

---

## 1️⃣9️⃣ Actions (CI/CD) 🤖

**GitHub Actions** = automated checks.

They:

* run tests
* check formatting
* block bad PRs

Your PR must pass Actions to merge.

---

## 2️⃣0️⃣ Checks

Checks show:

* ✔ passed
* ❌ failed
* ⏳ running

Failing checks = no merge.

---

## 2️⃣1️⃣ Status Badges

Small icons in README:

* build status
* coverage
* version

Shows project health.

---

## 2️⃣2️⃣ Commit

A saved change.

Good commit:

```
Fix crash on empty input
```

Bad commit:

```
fix
update
stuff
```

---

## 2️⃣3️⃣ Commit Squash

Multiple commits → one clean commit.

Used to:

* clean history
* simplify review

Often required before merge.

---

## 2️⃣4️⃣ Draft Pull Request

PR that is **not ready**.

Used when:

* work in progress
* want early feedback

---

## 2️⃣5️⃣ Templates

GitHub provides templates for:

* issues
* PRs

Forces contributors to include:

* steps
* expected behavior
* screenshots

---

## 2️⃣6️⃣ Mentions (@username)

Notify people.

Examples:

```text
@maintainer Can you review?
@team/frontend
```

---

## 2️⃣7️⃣ Notifications

You get notified when:

* someone comments
* review requested
* PR updated

Big projects = lots of notifications.

---

## 2️⃣8️⃣ Security Advisories

Used for:

* reporting vulnerabilities
* private discussion
* coordinated release

Never open public issues for security bugs.

---

## 2️⃣9️⃣ Releases

A **release** is a published version.

Includes:

* version number (v1.2.0)
* changelog
* assets

---

## 3️⃣0️⃣ Tags

Tags mark important commits.

Example:

```
v1.0.0
v2.1.3
```

Used for releases.

---

## 3️⃣1️⃣ Watch / Star / Fork

* ⭐ **Star** → show appreciation
* 👀 **Watch** → get updates
* 🍴 **Fork** → contribute

Stars matter for project visibility.

---

## 3️⃣2️⃣ Insights

Stats about:

* contributors
* commits
* activity
* code frequency

Used by maintainers.

---

## 3️⃣3️⃣ Maintainer

A **maintainer**:

* reviews PRs
* merges code
* sets direction

Be respectful. They’re often volunteers.

---

## 3️⃣4️⃣ Bot Accounts 🤖

Bots do:

* auto-merge
* auto-format
* dependency updates

Examples:

* Dependabot
* Renovate

---

## 3️⃣5️⃣ Permissions

Access levels:

* Read
* Write
* Maintain
* Admin

Most contributors have **Read only**.

---

