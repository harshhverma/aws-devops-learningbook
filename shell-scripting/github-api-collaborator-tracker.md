# GitHub Repository Collaborator Tracker using Shell Scripting

## Environment
- AWS EC2
- Shell Scripting
- GitHub API
- Linux Automation

---

# Project Overview

This project demonstrates how to automate the process of listing GitHub repository collaborators using shell scripting and GitHub APIs.

The automation helps DevOps engineers manage repository access efficiently without manually using the GitHub web interface.

---

# API vs UI

Most users interact with GitHub using the web UI.

DevOps engineers often use APIs for automation because APIs allow programmatic access to perform administrative and operational tasks efficiently.

---

# Environment Setup

## EC2 Instance
Used as the Linux environment for running shell scripts.

---

## GitHub Personal Access Token (PAT)

A Personal Access Token is used for authentication with GitHub APIs instead of using passwords.

Used for secure API access.

---

## Install JQ

`jq` is used to parse and filter JSON responses from APIs.

### Install jq
```bash
sudo apt install jq -y
```

---

# GitHub API Usage

The script uses `curl` to send API requests to GitHub.

## Example
```bash
curl -H "Authorization: token <TOKEN>" https://api.github.com
```

---

# JSON Parsing using JQ

GitHub API responses are returned in JSON format.

Use `jq` to extract useful data.

## Example
```bash
curl -s https://api.github.com/repos/OWNER/REPO/collaborators | jq '.[] | .login'
```

Used to list repository collaborator usernames.

---

# Script Workflow

The script performs the following tasks:

1. Connects to GitHub API
2. Authenticates using Personal Access Token
3. Fetches repository collaborators
4. Filters JSON response using jq
5. Displays usernames with repository access

---

# Real-World DevOps Use Case

This automation is useful for:

- Managing repository access
- Auditing GitHub permissions
- Removing access for former employees
- Team management automation
- Organization-wide repository monitoring

---

# Suggested Improvements

## Add Help Function

Provide usage instructions for users.

Example:
```bash
./script.sh <repo-owner> <repo-name>
```

---

## Add Comment Section

Document:
- Script purpose
- Author
- Usage
- Requirements

---

# Tools Used

- curl
- jq
- GitHub API
- Shell Scripting
- AWS EC2

---

# DevOps Relevance

This project demonstrates:

- API automation
- Infrastructure scripting
- Access management
- JSON parsing
- Linux shell scripting
- GitHub administration automation

---

# Key Takeaways

- Learned GitHub API basics
- Practiced API authentication
- Used curl for API requests
- Parsed JSON using jq
- Automated repository access tracking
- Understood real-world DevOps automation
