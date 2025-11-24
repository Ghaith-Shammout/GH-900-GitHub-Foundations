### Learning objectives
- [ ] Describe code scanning.
- [ ] List the steps for enabling code scanning in a repository.
- [ ] List the steps for enabling code scanning with third-party analysis.
- [ ] Contrast how to implement CodeQL analysis in a GitHub Actions workflow versus a third-party continuous integration (CI) tool.
- [ ] Explain how to configure code scanning on a repository using triggering events.
- [ ] Contrast the frequency of code scanning workflows (scheduled vs triggered by events).

## What is Code Scanning
Code scanning uses **CodeQL** to analyze the code in a GitHub repository to find **security vulnerabilities** and **coding errors**. Code scanning is available for all **public repositories**, and for **private repositories owned by organizations** where **GitHub Advanced Security** is enabled. 

If code scanning finds a potential vulnerability or error in your code, GitHub displays an alert in the repository's Security tab. After you fix the code that triggered the alert, GitHub closes the alert.

You can use code scanning to find, triage, and prioritize fixes for existing problems in your code. Code scanning also prevents developers from introducing new problems. You can schedule scans for certain days and times, or trigger scans when a specific event occurs in the repository, such as a push.

