# Introduction to GitHub

GitHub is a cloud-based platform built on top of Git that provides hosting for Git repositories along with collaboration tools, project management features, and social coding capabilities.


## Repository
A repository (or "repo") is a directory or storage space where your project lives. It contains all of your project's files and the entire history of changes made to those files.
What's actually in a repository:

1. Your project files - code, documentation, images, whatever your project needs
2. The .git directory - hidden folder containing all version control metadata, commit history, branch information, configuration
3. Commit history - complete record of every change, who made it, when, and why

Two types you need to distinguish:
- **Local repository** - exists on your machine. You can commit, branch, and work entirely offline.
- **Remote repository** - exists on a server (like GitHub). Acts as the central source of truth for team collaboration.

Once your repo is initiated on GitHub, now you are ready to clone your repo. 

### Cloning
Cloning creates a local copy of a repository on your machine. You use the command 
```bash
git clone <url>
```

- Creates a complete copy with all history on your local system
- Maintains a connection to the original repository (called the "remote" or "origin")
- You can pull updates from the original and push changes back (if you have permissions)
- Happens between GitHub (remote) and your computer (local)
- No new repository is created on GitHub

### Forking
Forking creates a copy of a repository under your own GitHub account.

- Happens entirely on GitHub's servers
- Creates a separate repository that you own and control
- The fork maintains a relationship to the original (upstream) repository
- You have full permissions on your fork even if you had none on the original
- Used primarily for contributing to projects you don't have write access to

**The key difference:**

Clone = GitHub → Your computer (download)

Fork = GitHub → GitHub under your account (server-side copy)

**Typical workflow for contributing to open source:**
- Step 1 - Fork the repository on GitHub (now you have your own copy)
- Step 2 - Clone your fork to your local machine
- Step 3 - Make changes locally
- Step 4 - Push changes to your fork
- Step 5 - Create a pull request from your fork to the original repository

## Gists

Gists are a GitHub feature for sharing small code snippets, notes, or files quickly without creating a full repository.

**What they are:**

- Lightweight repositories (yes, they're actually Git repositories under the hood)
- Designed for sharing individual files or small collections of files
- Can be public or secret (not private - important distinction)
- Each Gist gets its own URL
- Support version control - you can see edit history
- Can be forked, cloned, and embedded in web pages
- Support comments from other users

**Public vs Secret Gists:**

- **Public**: Discoverable, show up in search, appear on your profile
- **Secret**: Not discoverable or searchable, but NOT encrypted or truly private. Anyone with the URL can access it. Don't put passwords or sensitive data here.

**Common use cases:**

- Sharing code snippets in discussions or documentation
- Quick notes or to-do lists
- Configuration files you want to reference across machines
- Code examples for teaching or troubleshooting
- Embedding code snippets in blogs or websites

**What Gists are NOT:**

- Not a replacement for proper repositories with multiple collaborators
- Not secure storage (even secret Gists are accessible if someone has the link)
- Not meant for full projects with multiple directories and complex structure