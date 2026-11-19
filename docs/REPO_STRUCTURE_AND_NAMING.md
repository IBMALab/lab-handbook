# Repository Structure & Naming

## 1. One Repository per Student Project

Every project lives in **its own repository** inside the `Biomedical-Neurocomputing-Lab` organization.

```
Biomedical-Neurocomputing-Lab   (GitHub Organization)
│
├── lab-handbook                               ← this repo (rules & onboarding)
├── lab-project-template                       ← template for new projects
├── .github                                    ← org profile page
│
├── 2026-MS-ObaidullahM-EEG-Classification     ← one student, one project
├── 2026-BS-AyeshaK-Brain-Tumor-Segmentation
├── 2025-PhD-AliR-MRI-Super-Resolution
└── ...
```

**Rules**
- ✅ One repo = one project = one owner (student)
- ✅ Create repos **inside the organization**, never in your personal account
- ✅ If you work on two different projects, create two repos
- ❌ No shared "everyone's code" repository
- ❌ No folders like `ali/`, `ayesha/` inside a single repo

Shared/reusable lab code (e.g. common preprocessing utilities) goes in a separate
repo named `lab-<purpose>` (e.g. `lab-common-utils`), created **by the PI only**.

---

## 2. Naming Pattern

```
YYYY-DEGREE-StudentName-Topic
```

| Part | Rule | Example |
|------|------|---------|
| `YYYY` | Year the project started | `2026` |
| `DEGREE` | `BS` · `MS` · `PhD` · `PD` (postdoc) · `RA` (research assistant) | `MS` |
| `StudentName` | FirstName + LastName initial, CamelCase, no spaces | `ObaidullahM` |
| `Topic` | 1–4 short words, each capitalized, separated by `-` | `EEG-Classification` |

**Good ✅**
```
2026-MS-ObaidullahM-EEG-Classification
2026-BS-AyeshaK-Brain-Tumor-Segmentation
2025-PhD-AliR-MRI-Super-Resolution
2026-RA-HamzaS-Biomarker-Pipeline
```

**Bad ❌**
```
my-project                      → no year/degree/name
Obaidullah_FYP_final_v2         → underscores, "final", "v2"
2026 MS Obaidullah EEG          → spaces
2026-MS-ObaidullahMiakhil-Deep-Learning-Based-EEG-Signal-Classification-Using-CNN  → too long
```

**Group projects (e.g. BS FYP with 2–3 students):** use the group leader's name,
list all members in the README.
```
2026-BS-AyeshaK-Brain-Tumor-Segmentation
```

---

## 3. Standard Folder Layout (inside each project repo)

```
2026-MS-ObaidullahM-EEG-Classification/
├── README.md              ← required (use the template)
├── requirements.txt       ← Python dependencies  (or environment.yml)
├── .gitignore             ← copy from lab-handbook/templates/
├── code/                  ← all source code (.py / .m)
│   ├── preprocessing/
│   ├── models/
│   └── utils/
├── notebooks/             ← Jupyter notebooks (exploration only)
├── configs/               ← parameters, hyperparameters (.yaml / .json)
├── data/
│   └── README.md          ← WHERE the data is & how to get it — NOT the data itself
├── results/
│   ├── figures/           ← small final figures only
│   └── tables/
├── docs/                  ← thesis drafts, notes, slides (small files)
└── paper/                 ← LaTeX source of the paper (optional)
```

---

## 4. Repository Settings (set by the PI)

| Setting | Value |
|---------|-------|
| Visibility | **Private** until publication; public only with PI approval |
| Default branch | `main` (protected — changes only via Pull Request) |
| Team access | Student's team: **Write**; PI: **Admin** |
| Topics/tags | Add GitHub topics, e.g. `eeg`, `deep-learning`, `medical-imaging` |
| After graduation | Repo **archived**, student moved to `Alumni` team |

---

## 5. Making a Repo Public (after publication)

1. Paper accepted / thesis approved
2. Remove any sensitive data, paths, credentials (check full history)
3. Add a `LICENSE` (default: MIT for code) and a citation in README
4. PI approves and switches visibility to **Public**
5. PI pins it on the lab / PI profile
