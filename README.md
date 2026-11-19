# Biomedical-Neurocomputing-Lab — Lab Handbook

**Principal Investigator:** Dr. Muhammad Mohsin Khan, Associate Professor, PAF-IAST
**Research areas:** Biomedical imaging · AI/ML · Neurocomputing · Computing education

This repository is the single reference for how our lab writes, stores and shares code.
Every student must read it before creating their first project repository.

---

## 📌 The Core Rule: One Repository per Student Project

> **Do NOT put your work into one big shared repository.**
> Every student project gets **its own repository** inside the `Biomedical-Neurocomputing-Lab` organization.

Why:
- Clear ownership and history for each student's work
- Separate access control (private until published)
- Easy to archive when a student graduates
- Easy to link each repo to its thesis / paper

### Repository Naming Pattern

```
YYYY-DEGREE-StudentName-Topic
```

| Part | Meaning | Allowed values / format |
|------|---------|-------------------------|
| `YYYY` | Year the project **started** | e.g. `2026` |
| `DEGREE` | Program level | `BS`, `MS`, `PhD`, `PD` (postdoc), `RA` (research assistant) |
| `StudentName` | First name + last-name initial, no spaces | e.g. `ObaidullahM` |
| `Topic` | 1–4 words, each capitalized, hyphen-separated | e.g. `EEG-Classification` |

**Examples**

```
2026-MS-ObaidullahM-EEG-Classification
2026-BS-AyeshaK-Brain-Tumor-Segmentation
2025-PhD-AliR-MRI-Super-Resolution
2026-RA-HamzaS-Biomarker-Pipeline
```

Full details → [`docs/REPO_STRUCTURE_AND_NAMING.md`](docs/REPO_STRUCTURE_AND_NAMING.md)

---

## 📂 What's in this Handbook

| File | Purpose |
|------|---------|
| [`docs/ONBOARDING.md`](docs/ONBOARDING.md) | Step-by-step setup for new students |
| [`docs/REPO_STRUCTURE_AND_NAMING.md`](docs/REPO_STRUCTURE_AND_NAMING.md) | One-repo-per-project rule, naming pattern, folder layout |
| [`docs/CODING_RULES.md`](docs/CODING_RULES.md) | Coding, Git, data and reproducibility rules |
| [`templates/PROJECT_README_TEMPLATE.md`](templates/PROJECT_README_TEMPLATE.md) | README every project repo must have |
| [`templates/.gitignore`](templates/.gitignore) | Standard ignore file (Python + MATLAB + data) |
| [`templates/PULL_REQUEST_TEMPLATE.md`](templates/PULL_REQUEST_TEMPLATE.md) | PR checklist |

---

## ⚡ Quick Start (new student)

1. Read [`docs/ONBOARDING.md`](docs/ONBOARDING.md)
2. Accept the GitHub organization invitation
3. Create your repo from the **`lab-project-template`** using the naming pattern above
4. Fill in the README from the template
5. Commit at least **once per week**

---

## 🚫 Never Do This

- ❌ Push patient data, raw medical images or any identifiable data
- ❌ Push passwords, API keys or tokens
- ❌ Make a repo public without the PI's approval
- ❌ Delete or rename a repo yourself
- ❌ Work directly on `main` — use branches and pull requests

---

*Questions? Open an issue in this repository or contact the PI.*
