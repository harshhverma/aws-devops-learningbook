# Git & GitHub Fundamentals for DevOps

## Environment
- Git
- GitHub
- Version Control System (VCS)
- DevOps Workflow

---

# What is Version Control System (VCS)?

A Version Control System is used to track and manage changes made to source code over time.

It helps developers:
- collaborate in teams
- maintain version history
- restore previous versions
- track modifications safely

---

# Why Version Control is Important

Version control is important because:

- Multiple developers can work on same project
- Code history is maintained
- Bugs can be rolled back to stable versions
- Team collaboration becomes easier
- Prevents overwriting of code

---

# Centralized vs Distributed Version Control System

## Centralized VCS
Examples:
- SVN
- CVS

Characteristics:
- Single central server
- Developers depend on server availability
- Single point of failure

---

## Distributed VCS
Example:
- Git

Characteristics:
- Every developer has full local repository
- Work continues even if server is down
- Faster and more reliable collaboration

---

# What is Git?

Git is an open-source distributed version control system used to track code changes and maintain project versions.

---

# Why Git is Used in Real Projects

Git is used in real projects to:
- track source code changes
- support team collaboration
- manage feature development
- maintain code history
- enable rollback to previous stable versions

Git is heavily used in DevOps workflows and CI/CD pipelines.

---

# What is GitHub?

GitHub is a cloud-based platform built on top of Git used to host repositories and enable collaboration among developers.

It provides:
- repository hosting
- issue tracking
- pull requests
- project management
- collaboration features

---

# Difference Between Git and GitHub

| Git | GitHub |
|---|---|
| Version control tool | Cloud hosting platform |
| Works locally | Works online |
| Tracks code changes | Hosts repositories and collaboration |

---

# What is Fork?

Fork creates a personal copy of another repository inside your own GitHub account.

Used mainly for:
- open source contribution
- experimentation
- independent development

---

# Difference Between Fork and Clone

| Fork | Clone |
|---|---|
| GitHub to GitHub copy | GitHub to local machine copy |
| Used for contribution | Used for local development |

---

# Git Workflow

```text
Working Directory
       ↓
git add
       ↓
Staging Area
       ↓
git commit
       ↓
Local Repository
       ↓
git push
       ↓
GitHub Repository
```

---

# Important Git Commands

## Initialize Repository

```bash
git init
```

Used to start version tracking in a project.

---

## Check Repository Status

```bash
git status
```

Displays:
- modified files
- staged files
- untracked files

---

## Add Files to Staging Area

```bash
git add .
```

Used to prepare changes before committing.

---

## Commit Changes

```bash
git commit -m "Initial commit"
```

Creates a snapshot/version of the project.

---

## View File Differences

```bash
git diff
```

Shows modifications between versions.

---

## View Commit History

```bash
git log
```

Displays commit history and commit IDs.

---

## Revert Changes

```bash
git reset
```

Used to undo staged changes or move back to previous commits.

---

# Why Git is Important in DevOps

Git is one of the most important tools in DevOps because it enables:

- CI/CD integration
- Infrastructure as Code versioning
- Deployment automation
- Team collaboration
- Rollback and recovery
- Source code management

---

# Key Takeaways

- Understood Version Control Systems
- Learned centralized vs distributed VCS
- Understood Git vs GitHub
- Learned Git workflow
- Practiced important Git commands
- Understood practical DevOps usage of Git
