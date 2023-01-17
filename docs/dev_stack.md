
!!! Abstract 

	The Iterative Website Development Stack illustrates how websites are developed by teams and deployed to the Internet. It is web browser agnostic. What works for big screens, works for small screens.


---

### Dev Stack
<div style="text-align: center;">


``` mermaid
flowchart TB
	
	crepo --- cdn

	cdn --- net

	dev --- vsc 

	github --- crepo

	github --- net
	
	vsc --- lrepo
	
	net --- prevweb

	net --- proweb

	vsc --- net

	vsc --- mkd

	mkd --- lpreweb

	dev([Team Developers])

	cdn([CDN - Deploy Project to Web])

	crepo([Central Project Repository])

	github([GitHub]) 

	lrepo([Local Projet Repository])

	lpreweb([Local Preview Website])

	mkd([Mkdocs Material - Static Site Generator])

	net([Internet]) 
	
	prevweb([Stake Holders Private Preview Website])

	proweb([Production Website])

	vsc([VScode - Command and Control]) 

```
<b>Iterative Website Development Stack</b>
</div>


>The core technologies of Iterative Development are Git, GitHub, and the Central Project Repository controlled by the project gatekeeper, and a content delivery network, like Cloudflare, deploying private Preview Internet websites, production websites, and individual team members private Preview websites.
>

>GitHub is a Distributed Version Control Systems enabling multiple teams to work separately on the same project without having an impact on the work of others. GitHub manages an online web hosted central project repository containing all project files. It is a unified source of truth. It helps teams collaborate and maintain the entire history of project file changes.

>The Central Repository is managed my a team member

>It helps answer the questions for the lifetime of the project **who changed what, where, when, and why?** for the lifetime of the project

---

> Team members use the Website Development Stack to develop, deploy, and maintain websites to the Internet. 

>There would be confusion and possible defects created if Team members were to directly make changes to the central project repository.  

>A solution to this problem is to have one central repository controlled by a team member gatekeeper. Each team member [forks](git-github#fork) a copy of central project repository to their GetHub account and makes a [clone](glossary#clone) of it on their workstation.

>Each developer makes changes to their repository [clone](glossary#clone). They cannot directly make changes to the central repository.



The Iterative Development teams use the Iterative Website Development Stack technologies

The core technologies are [VScode](), [Git](), [GitHub](dev_stack_details#github-details) and the *Central Project Repository* controlled by the project gatekeeper,  using Local Website Repository, the content delivery network, like Cloudflare, to deploying private [Preview](preview.md) Internet websites, production websites, and .


#### Team Developers 

- Local Website Repository   
	Each team developer has their own Local Website Repository that can be updated from the Central Website Repository. Team members cannot update the Central Web Repository directly. They submit their changes. The approved changes by the project gatekeeper are added to the Central Website Repository. Team members can then update their Local Website Repositories.

- VScode   
	Developers use [VSCode](vscode.md) as their Web Development Stack Command and Control center. They use it to edit code using their Local Website Repository, commit changes to the Central Website Repository, refresh their Local Website Repository, and deploy [Preview](preview.md) Internet for themselves and stakeholders to view and give feedback



---

#### GitHub

[GitHub](github.md) is a Distributed Version Control Systems enabling multiple teams to work separately on the same project without having an impact on the work of others. GitHub manages an online web hosted Central Website Repository containing all project files. It is a unified source of truth. It helps teams collaborate and maintain the entire history of project file changes, and helps answer the questions **who changed what, where, when, and why** for the lifetime of the project

#### GitHub Central Repository.  

The core technologies of Iterative Development SCM are Git, GitHub, and the Central Website Repository controlled by the project gatekeeper, and a content delivery network, like Cloudflare, deploying private Preview Internet websites, production websites, and individual team members private Preview websites.

The Central Website Repository is managed by a team member project gatekeeper with help from other team members

---

#### GitHub Workflow

- GitHub workflow is centered on [Pull](git.com#pull) git command. The GitHub workflow works with collaborating team members contributing to the central project repository using the [Fork](git.md#fork) command It is centered on the topic Branches workflow.

A summary of GitHub workflow for each team member is:

  1. [Fork](git.md#fork) the central project repository creating a local project repository in individual team members GitHub account
  2. [Clone](git.md#clone) the forked local project repository in team member GitHub account to workstation
  3. Creates a topic [Branch](git.md#branch) off the cloned local project repository **main** branch
  4. Make topic edits and commits 
  5. [Push](git.md#push) after each commit to the cloned local project repository in GitHub account
  6. Periodically [Pull](git.md#pull) from the central project repository. The **develop** branch will have merged accepted Pull Requests
  7. Periodically deploy local project repository to a private [Preview ](preview.md) website without disturbing other developers work or the production version, for stake holders viewing and feedback. This reduces the Pull Request evaluation time because stake holders interested in topics can see how they are progressing and working with the website.
  8. Open a [Pull](git.md#pull) Request on the GitHub local project repository to begin the  process of integrating the local project repository with the central project repository  
  9. Team members discuss, and optionally continue committing on Pull Requests.

---


- Reference [GitHub Details](dev_stack_details#github_details)

#### MkDocs Material - Static Site Generator

Is a Static Site Generator used to build a website from a repository to create:
  
  - Developers use it and their local repository to [Preview](preview.md) how features, fixes, experimental ideal, they are working on will possible look on the website

  - Content Delivery network(CDN) uses it create [Preview](preview.md)Stake Holders 

It is also used by the  do build and deploy the production website from the Central Repository



#### Content Delivery Network (CDN)



  
A "MkDocs Static Site Generator" tools are used to create the "Production Website" by the "CDN - Deploy Website to Web"


### GitHub 
Central Repository.  

>The core technologies of Iterative Development are Git, GitHub, and the Central Website Repository controlled by the project gatekeeper, and a content delivery network, like Cloudflare, deploying private Preview Internet websites, production websites, and individual team members private Preview websites.
>

>GitHub is a Distributed Version Control Systems enabling multiple teams to work separately on the same project without having an impact on the work of others. GitHub manages an online web hosted central project repository containing all project files. It is a unified source of truth. It helps teams collaborate and maintain the entire history of project file changes.

>The Central Repository is managed my a team member

>It helps answer the questions for the lifetime of the project **who changed what, where, when, and why?** for the lifetime of the project

---

> Team members use the Website Development Stack to develop, deploy, and maintain websites to the Internet. 

>There would be confusion and possible defects created if Team members were to directly make changes to the central project repository.  

>A solution to this problem is to have one central repository controlled by a team member gatekeeper. Each team member [forks](git-github#fork) a copy of central project repository to their GetHub account and makes a [clone](glossary#clone) of it on their workstation.

>Each developer makes changes to their repository [clone](glossary#clone). They cannot directly make changes to the central repository.

- Team members commit changes to their local repository clone

- They may deploy their local repository to a private [Preview](preview.md) Internet website for stakeholders to see and give feedback. 

- The process is managed using [GitHub for Teams](https://github.com/team). When stakeholders determine developers changes, defect fixes, or new features are ready, a GitHub [Pull Request](git-github#pull-request) is made by developers to the central project repository. 

	- Project team members and the gatekeeper are notified by GitHub of the [Pull Request](git-github#pull-request) request. They may examine, comment on, suggest possible changes, and test the code. 

	- When the team agrees on committed developers changes, they are committed to the central project repository by the gatekeeper. This process is repeated for all developer committed changes. 

	- Iterations of the central project repository may be deployed by the gatekeeper to a private [Preview](preview.md)  for stakeholders viewing. 

- The next step is each developer [Pulls](git-github#pull) the central repository changes and commits them to their local repository copy of the central project. This process keeps team members up to date on changes.

- The central project repository may be deployed to the public Internet by the gatekeeper after stakeholders agree there have been sufficient development and testing iterations.

