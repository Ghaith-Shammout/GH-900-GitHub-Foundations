GitHub Codespaces is an instant, cloud-based development environment that uses a container to provide you with common languages, tools, and utilities for development.
GitHub Codespaces is configurable, allowing you to create a customized development environment for your project.
By configuring a custom development environment for your project, you can have a repeatable Codespace configuration for all users of your project.


### The Codespace lifecycle

The **GitHub Codespaces lifecycle** describes the stages a codespace goes through from creation to deletion. Here’s a clear breakdown:

***

### **1. Creation**

*   You start by creating a codespace from a GitHub repository (via the GitHub UI, CLI, or API).
*   GitHub provisions a **virtual machine** in the cloud and sets up the environment based on:
    *   The repository’s **dev container configuration** (`.devcontainer/devcontainer.json`).
    *   Default settings if no configuration exists.

You can create a Codespace:
* From a GitHub Codespaces template (or any template repo) – for starting a brand‑new project. [GitHub](https://docs.github.com/en/codespaces/developing-in-a-codespace/creating-a-codespace-from-a-template)
* From a branch in a repository – the standard “Code → Codespaces → New codespace” flow lets you pick the branch. [GitHub](https://docs.github.com/en/codespaces/developing-in-a-codespace/creating-a-codespace-for-a-repository)
* From an open pull request – GitHub adds a Codespaces button on PRs to open a codespace on the PR’s topic branch. [docs.github.com]

***

### **2. Initialization**

*   The codespace installs all required dependencies and tools defined in the dev container.
*   It sets up the editor (VS Code) and extensions.
*   This step ensures the environment matches the project requirements.

***

### **3. Active / Running**

*   You can **open the codespace** in:
    *   Browser (web-based VS Code)
    *   Local VS Code (via remote connection)
*   During this stage, you:
    *   Write code
    *   Run tests
    *   Debug applications
*   The codespace runs on a **remote VM**, but feels like local development.

***

### **4. Suspension**

*   If you stop working or close the codespace, it enters a **suspended state**.
*   The VM is paused, and your work is saved.
*   This helps reduce costs while keeping the environment ready for quick resume.

***

### **5. Resumption**

*   When you reopen the codespace, it resumes from the suspended state.
*   No need to reinstall dependencies—everything is preserved.

***

### **6. Deletion**

*   You can delete a codespace manually or let it expire based on **retention policies**.
*   Once deleted:
    *   The VM and its data are removed.
    *   GitHub may keep logs for auditing, but your workspace is gone.

***

✅ **Key Benefit:** This lifecycle ensures **fast startup**, **consistent environments**, and **cost efficiency** by suspending unused codespaces.

***

Would you like me to **illustrate this lifecycle with a diagram** or **compare it to Docker container lifecycle for better understanding**?
