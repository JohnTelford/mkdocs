---
title: Dev Stack Details
---


## GitHub and Git Details

- A Distributed Version Control Systems enabling multiple teams to work separately on the same project without having an impact on the work of others. GitHub manages an online web hosted Central Website Repository containing all project files. 

- It is a unified source of truth. It helps teams collaborate and maintain the entire history of project file changes, and helps answer the questions who changed what, where, when, and why for the lifetime of the project

### GitHub Workflow

- GitHub workflow is centered on Pull Request The GitHub workflow works with collaborating team members contributing to the central project repository using the Forks. It is centered on the topic Branches workflow.

A summary of GitHub workflow for each team member is:

  1. [Fork](https://www.w3schools.com/git/git_remote_fork.asp?remote=github) the central project repository creating a local project repository in individual team members GitHub account
  2. [Clone](https://www.w3schools.com/git/git_clone.asp?remote=github) the forked local project repository in team member GitHub account to workstation
  3. Creates a topic Branch off the cloned local project repository *main* branch
  4. Make topic edits and commits 
  5. [Push](https://www.w3schools.com/git/git_push_to_remote.asp?remote=github) after each commit to the cloned local project repository in GitHub account
  6. Periodically [Pull](https://www.w3schools.com/git/git_push_to_remote.asp?remote=github) from the central project repository. The *develop* branch will have merged accepted Pull Requests
  7. Periodically deploy local project repository to a private [Preview ](preview.md) website without disturbing other developers work or the production version, for stake holders viewing and feedback. This reduces the Pull Request evaluation time because stake holders interested in topics can see how they are progressing and working with the website.
  8. Open a Pull Request on the GitHub local project repository to begin the  process of integrating the local project repository with the central project repository  
  9. Team members discuss, and optionally continue committing on Pull Requests.

---

### Git Details

- Git is not the same as GitHub.
- GitHub makes tools that use Git.### The Project Gatekeeper 
	
- Merges or closes Pull Requests to the central project repository, and deploys the central project repository to a private [Preview ](deploy#preview) website for stack holders viewing. The teams and gatekeeper continues the GitHub workflow process until stack holders agree the central project repository is ready for release to the public internet 

- Teams may Pull the central project repository at anytime to view and test other topic branches.



#### Reference

- [What is Git and GitHub](https://www.w3schools.com/git/default.asp)
- [GitHub](https://github.com/)
- [Git](https://git-scm.com/)

---

### VScode

[Introduction Videos](https://code.visualstudio.com/docs/getstarted/introvideos)
