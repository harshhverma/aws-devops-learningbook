# Git Branching Strategy for DevOps

## Environment
- Git
- GitHub
- Version Control
- DevOps Workflow

---

# What is a Branch in Git?

A branch is a separate workspace in Git that allows developers to work independently without affecting the stable production code.

Branches help teams:
- develop features safely
- test new functionality
- fix bugs independently
- collaborate efficiently

---

# Why Branching is Important

Branching is important because:

- Multiple developers can work simultaneously
- Production code remains stable
- New features can be tested safely
- Bugs can be fixed independently
- Releases become more organized and reliable

---

# Real-World Example

Suppose an application currently supports:
- Cab booking

Now developers want to add:
- Bike booking
- Intercity rides

Instead of directly modifying stable production code, developers create separate branches for these features.

This prevents unstable code from affecting existing users.

---

# Main Types of Git Branches

---

# 1 Master / Main Branch

The Main branch contains:
- stable code
- production-ready application
- latest working version

Characteristics:
- should always remain stable
- used for production deployments
- acts as primary source of truth

---

# 2️ Feature Branch

Feature branches are created to develop new features independently.

Examples:
- login-feature
- payment-feature
- search-feature

Workflow:
1. Create feature branch
2. Develop feature
3. Test feature
4. Merge back into main branch

---

# 🔹 Why Feature Branches are Used

Feature branches help:
- isolate development
- avoid breaking production code
- support parallel development
- simplify testing and code reviews

---

# 3️ Release Branch

Release branches are used to prepare a specific software version for deployment.

While testing occurs on release branch:
- development can continue on main branch

Used for:
- final testing
- bug verification
- deployment preparation

---

# Why Release Branches are Important

Release branches help organizations:
- stabilize releases
- avoid delaying development
- ensure predictable deployments

---

# 4️ Hotfix Branch

Hotfix branches are temporary branches used to fix critical production issues quickly.

Example:
- payment failure
- server crash
- security issue

After fixing:
- changes merged into main branch
- changes merged into release branch

---

# Why Hotfix Branches are Important

Hotfix branches help:
- resolve production bugs quickly
- avoid disturbing ongoing development
- maintain application stability

---

# Basic Git Branch Workflow

```text
Main Branch
     ↓
Create Feature Branch
     ↓
Develop & Test Feature
     ↓
Merge into Main Branch
     ↓
Create Release Branch
     ↓
Deploy to Production
```

---

# Common Git Branch Commands

## View Branches

```bash
git branch
```

---

## Create New Branch

```bash
git branch feature-login
```

---

## Switch Branch

```bash
git checkout feature-login
```

---

## Create and Switch Together

```bash
git checkout -b feature-login
```

---

## Merge Branch

```bash
git merge feature-login
```

---

# Real DevOps Relevance

Branching strategies are important in DevOps because they help:
- manage large teams
- support CI/CD pipelines
- maintain production stability
- enable parallel development
- simplify deployments

---

# Kubernetes Real-World Example

Large open-source projects like Kubernetes use branching strategies to manage:
- thousands of contributors
- multiple releases
- production stability
- bug fixes and new features simultaneously

---

# Interview Questions & Answers

## 1️ What is a Git Branch?

A Git branch is an independent line of development used to work on features or fixes without affecting the main stable codebase.

---

## 2️ Why are Branches Used in Git?

Branches are used to isolate development work, support collaboration, and prevent unstable code from affecting production.

---

## 3️ What is a Feature Branch?

A feature branch is a temporary branch used to develop and test a specific feature independently.

---

## 4️ What is a Release Branch?

A release branch is used to prepare and stabilize a specific software version before deployment.

---

## 5️ What is a Hotfix Branch?

A hotfix branch is a temporary branch created to quickly fix critical production issues.

---

## 6️ Why is Branching Strategy Important in DevOps?

Branching strategies help teams manage code safely, support CI/CD pipelines, maintain stable releases, and improve collaboration.

---

# Key Takeaways

- Learned Git branching concepts
- Understood feature, release, and hotfix branches
- Learned importance of stable production code
- Understood real-world DevOps collaboration workflow
- Learned practical Git branch commands
