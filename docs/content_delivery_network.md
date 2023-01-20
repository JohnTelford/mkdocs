
### CDN

---

## Branch build controls

[Branch build controls](https://developers.cloudflare.com/pages/platform/branch-build-controls/)

When connected to your git source, Pages allows you to control which environments and branches you would like to automatically build. By default, Pages will trigger a build any time you commit to either your production or preview environment. However, with branch build controls, you can configure automatic deployments to suit your preference on a per project basis.

### Skip builds

[Skip builds](https://developers.cloudflare.com/pages/platform/branch-build-controls/#skip-builds)

Without any configuration required, you can choose to skip a build and deployment on an adhoc basis. By adding the [CI Skip], [CI-Skip], [Skip CI], [Skip-CI] or [CF-Pages-Skip] flag as a prefix in your commit message, Pages will omit that build/deployment. The prefixes are case insensitive.

### Production branch control

[Production branch control](https://developers.cloudflare.com/pages/platform/branch-build-controls/#production-branch-control)

To configure deployment options, go to your Pages project > Settings > Builds & deployments > Configure Production deployments. Pages will default to setting your production environment to the branch you first push, but you can set your production to another branch if you choose.


### Preview branch control

[Preview branch control](https://developers.cloudflare.com/pages/platform/branch-build-controls/#preview-branch-control)

When configuring automatic builds for preview deployments, there are three options to choose from.

- All non-Production branches: By default, Pages will automatically deploy any and every commit to a preview branch.
- None: Turns off automatic builds for all preview branches.
- Custom branches: Customize the automatic deployments of certain preview branches.

### Custom preview branch control
https://developers.cloudflare.com/pages/platform/branch-build-controls/#custom-preview-branch-controlhttps://developers.cloudflare.com/pages/platform/branch-build-controls/#custom-preview-branch-control

Custom preview branch control

By selecting Custom branches, you can specify branches you wish to include and exclude from automatic deployments in the provided configuration fields. The configuration fields can be filled in two ways:

- Static branch names: Enter the precise name of the branch you are looking to include or exclude (for example, staging or dev).

- Wildcard syntax: Use wildcards to match multiple branches. You can specify wildcards at the start or end of your rule. The order of execution for the configuration is:
	- Excludes
	- Includes
	- Skip
	
Pages will process the exclude configuration first, then go to the include configuration. If a branch does not match either then it will be skipped.

### Wildcards

[Wildcards](https://developers.cloudflare.com/pages/platform/branch-build-controls/#wildcards)

A wildcard (*) is a character that is used within rules. It can be placed alone to match anything or placed at the start or end of a rule to allow for better control over branch configuration. A wildcard will match zero or more characters.

For example, if you wanted to match all branches that started with fix/ then you would create the rule fix/* to match strings like fix/1, fix/bugsor fix/.

---

## Preview deployments

[Preview Deployment](https://developers.cloudflare.com/pages/platform/preview-deployments/)

Preview deployments allow you to preview new versions of your project without deploying it to production. To view preview deployments, navigate from the Account Home Pages and select your project
 
### Customizing preview deployments access 
 
 [Customizing preview deployments access](https://developers.cloudflare.com/pages/platform/preview-deployments/#customizing-preview-deployments-access)
 
 You can use Cloudflare AccessOpen external link to manage access to your deployment previews. By default, these deployment URLs are public. Enabling the access policy will restrict viewing project deployments to your Cloudflare account.

### Preview aliases

[Preview aliases](https://developers.cloudflare.com/pages/platform/preview-deployments/#preview-aliases)

When a preview deployment is published, it is given a unique, hash-based address — for example, <hash>.<project>.pages.dev. These are atomic and may always be visited in the future. However, Pages also creates an alias for git branch’s name and updates it so that the alias always maps to the latest commit of that branch.

