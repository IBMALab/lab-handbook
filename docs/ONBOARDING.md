# Onboarding — New Student Setup

Complete every step in your **first week** in the lab. Tick them off as you go.

---

## Step 1 — GitHub Account
- [ ] Create a GitHub account (or use your existing one)
- [ ] Use a **professional username** (e.g. `obaidullah-miakhil`, not `gamer_boy99`)
- [ ] Add your real name and profile photo
- [ ] Add your **university email** to the account (Settings → Emails)
- [ ] Enable **two-factor authentication** (Settings → Password and authentication) — required
- [ ] Optional: apply for the free **GitHub Student Developer Pack** at <https://education.github.com>

## Step 2 — Join the Lab Organization
- [ ] Send your GitHub username to the PI
- [ ] Accept the invitation to `IBMALab` (check your email or <https://github.com/orgs/IBMALab/invitation>)
- [ ] Confirm you've been added to your team (e.g. `MS-2026`, `BS-FYP-2026`)

## Step 3 — Install Tools
- [ ] **Git** — <https://git-scm.com/downloads>
- [ ] **VS Code** (recommended) — <https://code.visualstudio.com>
- [ ] **Python 3.10+** via Anaconda/Miniconda, and/or **MATLAB** (as your project needs)
- [ ] Optional: **GitHub Desktop** if you are new to Git

Configure Git once:
```bash
git config --global user.name  "Your Full Name"
git config --global user.email "your-university-email@example.edu"
git config --global init.defaultBranch main
```

## Step 4 — Connect to GitHub (SSH, recommended)
```bash
ssh-keygen -t ed25519 -C "your-university-email@example.edu"
# Copy the public key:
cat ~/.ssh/id_ed25519.pub
```
Paste it in GitHub → Settings → **SSH and GPG keys** → New SSH key. Test:
```bash
ssh -T git@github.com
```

## Step 5 — Create Your Project Repository
1. Go to the org's **`lab-project-template`** repo → **Use this template → Create a new repository**
2. **Owner:** `IBMALab` (⚠️ NOT your personal account)
3. **Name:** follow the pattern `YYYY-DEGREE-StudentName-Topic`
   → e.g. `2026-MS-ObaidullahM-EEG-Classification`
4. **Visibility:** **Private**
5. Clone it:
```bash
git clone git@github.com:Biomedical-Neurocomputing-Lab/2026-MS-ObaidullahM-EEG-Classification.git
```
6. Fill in `README.md` using [`templates/PROJECT_README_TEMPLATE.md`](../templates/PROJECT_README_TEMPLATE.md)
7. Ask the PI to confirm the repo name — **don't rename it later yourself**

## Step 6 — Read the Rules
- [ ] [`REPO_STRUCTURE_AND_NAMING.md`](REPO_STRUCTURE_AND_NAMING.md)
- [ ] [`CODING_RULES.md`](CODING_RULES.md) — especially the **data policy**

## Step 7 — First Commit
```bash
git checkout -b setup/initial-readme
# edit README.md
git add README.md
git commit -m "docs: add project README"
git push -u origin setup/initial-readme
```
Then open a **Pull Request** on GitHub and request a review from the PI.

---

## Git Basics You Will Use Daily

| Task | Command |
|------|---------|
| Get latest changes | `git pull` |
| New branch | `git checkout -b feature/short-name` |
| See what changed | `git status` |
| Stage files | `git add <file>` |
| Commit | `git commit -m "type: message"` |
| Upload | `git push` |

Learning resources:
- GitHub Skills (interactive): <https://skills.github.com>
- Pro Git book (free): <https://git-scm.com/book>

---

## When You Leave / Graduate
- [ ] Final code, README and results are pushed
- [ ] README links to your thesis / paper
- [ ] All open branches merged or closed
- [ ] PI archives the repo and moves you to the `Alumni` team (read-only access to your work remains)
