# Checkpoint 5 — Final Integrated GitHub Challenge

## Goal

Prove that you can create a project **from scratch** and carry it through a complete Git/GitHub team workflow independently.

CP5 integrates:

```text
repository setup
→ local Git workflow
→ Issue
→ Project/Kanban
→ feature branch
→ Pull Request
→ self-check
→ merge
→ Done
→ debugging / recovery
```

## Start CP5 — do NOT copy this repository

This KLIS-CS repository is the **instruction and grading portal only**.

Create a new **Public** repository in your own GitHub account with **GitHub → New repository**. Do not fork and do not use **Use this template**.

Required repository name:

```text
cp5-final-integrated-YOUR-GITHUB-USERNAME
```

When creating it, configure:

- `README.md`
- an appropriate `.gitignore`
- a real open-source `LICENSE`
- default branch `main`

## Scenario

Your team needs a JavaScript feature that displays a welcome message. You are responsible for planning the work, implementing it safely, self-checking it, merging it, and closing the work item.

## Required workflow

### 1. Create and inspect the repository

Clone your new repository and inspect it before changing anything:

```bash
git status
git branch -vv
git remote -v
```

### 2. Create one GitHub Project

Create **one GitHub Project** with a **Board** view and these exact statuses:

```text
Todo → In Progress → Review → Done
```

This Project must track both the CP5 Issue and the CP5 Pull Request.

### 3. Create the work Issue

Create an Issue whose title begins with `[CP5]`.

It must:

- clearly describe the feature;
- include at least two acceptance-criteria checkboxes;
- have at least one label;
- be assigned to you.

Add the Issue to the Project in **Todo**, then move it to **In Progress** when implementation begins.

### 4. Implement through a feature branch

Create this branch locally:

```text
cp5-YOUR-GITHUB-USERNAME
```

Do not implement the feature directly on `main`.

On the feature branch:

- create `src/index.js`;
- add working JavaScript that produces or displays a welcome message;
- make at least one meaningful improvement to `README.md`;
- use `git status` before staging;
- stage only intended changes;
- commit with a meaningful message;
- push the branch to `origin`.

### 5. Open the Pull Request and move to Review

Open a Pull Request from `cp5-YOUR-GITHUB-USERNAME` → `main`.

The PR body must connect to the CP5 Issue with a closing keyword, for example:

```text
Closes #12
```

Then:

1. add the PR to the **same GitHub Project**;
2. move both Issue and PR to **Review**;
3. inspect your own Pull Request and leave a clear **self-check message** in the PR Conversation, such as `Self-check complete: files, Issue link, and submission verified. Ready to merge.`

### 6. Merge and finish

After approval:

1. merge the Pull Request into `main`;
2. confirm the linked Issue closes;
3. move both Issue and PR to **Done**.

Do not merge before your self-check message. The grader compares the message timestamp with the merge timestamp.

Deleting the feature branch after merge is allowed. The Pull Request keeps the head ref/SHA and Conversation history needed for grading.

### 7. Debugging / recovery

The submission form includes recovery scenarios covering:

- accidentally editing on `main`;
- a file missing from a commit;
- a branch with no upstream;
- an incorrect remote URL.

Explain what you would inspect first and how you would recover safely.

## Submit CP5

Submit only after the self-checked PR is merged and the Project is in its final state:

[![Submit CP5](https://img.shields.io/badge/SUBMIT%20CP5-%E2%86%92-0969da?style=for-the-badge&logo=github)](https://github.com/KLIS-CS/GitHub-Final-Integrated-Challenge/issues/new?template=cp5-submission.yml)

The repository URL and GitHub username are detected automatically.

The **same CP5 Submission Issue** is the single source of truth for grading. Its score comment is updated in place with:

- Automatic score `/60`
- Teacher score `/40`
- Final score `/100`
- Teacher feedback

## Automatic evidence — 60 points

| Evidence | Points |
|---|---:|
| Correct public student-owned repository created from scratch | 10 |
| Meaningful README / `.gitignore` / LICENSE / `src/index.js` | 10 |
| Correct feature-branch and PR change/commit evidence | 10 |
| `[CP5]` Issue quality and closure after merge | 10 |
| PR links Issue, contains the student's self-check message before merge, and is merged | 10 |
| Complete Project/status, concepts, debugging, and reflection submission | 10 |
| **Automatic subtotal** | **60** |

## Teacher review — 40 points

Teacher review focuses on:

- workflow independence;
- Project/Kanban evidence;
- conceptual understanding;
- debugging / recovery reasoning;
- reflection and work quality.

For full **Project evidence**, verify:

- Board has **Todo / In Progress / Review / Done**;
- the CP5 Issue and CP5 Pull Request are in the **same Project**;
- both finish in **Done**;
- the workflow reflects a sensible progression, not only a final-state setup.

Teacher grading format:

```text
/manual-grade
Workflow independence: 0/10
Project evidence: 0/5
Concepts: 0/10
Debugging: 0/10
Reflection: 0/5

Feedback:
Write concise feedback here.
```

Students do **not** need to add grading workflows to their own CP5 repository or run Actions manually.

## Checkpoint Navigation

| Checkpoint | Skill | Link |
|---|---|---|
| CP1 | Repository Setup | [Open](https://github.com/KLIS-CS/GitHub-Repository-Setup) |
| CP2 | Feature Branch & Pull Request | [Open](https://github.com/KLIS-CS/GitHub-Feature-Branch-Pull-Request-Workflow) |
| CP3 | Issues & Projects | [Open](https://github.com/KLIS-CS/GitHub-Issues-Projects-Workflow) |
| **CP5 — You are here** | Final Integrated Challenge | [Open](https://github.com/KLIS-CS/GitHub-Final-Integrated-Challenge) |

[Back to GitHub Foundations Hub](https://github.com/KLIS-CS/GitHub-Foundations)
