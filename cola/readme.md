# Github Basics

## Version Control Systems (VCS)
Designed to track changes or revisions to code.

## GitHub
- Well-based interface accessed via browser
- Accessible anywhere with internet
- Directly manage repositories online
- Perform operations like fork, star, watch
- Direct collaboration tools like issues, pull requests
- Supports advanced features via commands
- Integrates with various online CI/CD tools
- Version Control as a Service (VCaaS)
- Provides cloud storage for git repositories
- Acessed via will interface
- Online collaboration and repository hosting
- Integrated tools for collaboration
- Graphical interface and additional features
- Version Control Service (VCS)
- Git Repository Hosting
- Project Management Tools
- Issue Tracking
- Pull Requests and Code Review
- Pages and Wikis
- Actions
- Copilot
- Codespaces
- Marketplace
- Gists
- Discussions
- Collaborations Features
- API Acess and Development Tools
- Security Features
- Educational Resources and Course Automation

## Git
Distributed Version Control System (DVCS)
- Manages source code history
- Local system installation
- Local repository management
- Local changes, manual sharing
- Command-line interface

## Common Git Terms
- Repository
- Commit
- Tree
- Remote
- Branches
- Clone
- Checkout
- Pull
- Push
- Fetch
- Reset
- Merge
- Staging

## VCS
Fully managed cloud services that hosts your version controlled repositories
- Github
- Gitlab
- BitBucket
- SourceForge

## Github Repo
Your git repo that you push upstream to Github
```gh
git init
```

### Cloning
We can clone three ways:
- HTTPS
- SSH
- Github CLI
```gh
git clone
```
### Git Hidden Folder
Hidden folder called .git which tells you that our project is a git repo

### Add
When we want to stage changes that will be included in the commit
```gh
git add .
git add [file]
```

### Reset
Allows you to move staged changes to be unstaged
```gh
git reset
```

### Status
Git status shows you what files will or will not be commited.
```
git status
```

### Commit
When we want to commit code
- Commit Hash
- Author Information
- Commit Message
- Timestamp
- Parent Commit Hash
- Snapshot of content
```gh
git commit -m "message"
git commit  -a -m "message"
git commit --amend
git commit -m "Initial commit" --allow-empty
```

### Git config file
Is what stores your global configurations for git such as email, name and more
```gh
git config
```

### Log
Will show recent git commits to the git tree
```gh
git log
```

### Push
When we want to push a repo to our remote origin
```gh
git push
```

### Pull
```gh
git pull
```

### SSH
- Common strategy for authenticating to perform git operations
- SSH uses a public and private key to authorize remote access to servers
```
ssh-keygen -t rsa
```

### Branches
**A divergence of the state of the repo**
- Branches can be created from Issues
- Branches can be directly created within Github UI
- Branches can be created in Github Desktop
- using git we can create a new branch from an existing branch
```gh
git branch
git branch -a
git branch [branch-name]
git branch -d [branch-name]
git branch -m [old-name][new-name]
git checkout [branch-name]
git checkout -b [branch-name]
```

### Remotes
Represents the reference to remote location
```gh
git remote -v
git remote add [name][URL]
git remote remove [name]
git remote rename [old-name][new-name]
git push [remote-name][branch]
git pull [remote-name][branch]
git fetch [remote-name][branch]
```

### Stashing
```gh
git stash [...]
```

### Merging
```gh
git merge [branch-name]
```
## Github Flow
light-weight workflow for multiple developers working on a single repository
1. create branch
2. add commits
3. open a pull request
4. discuss and review
5. deploy
6. merge

## Github CLI
Command line interface to interact with you Github account
```gh
gh [...]
```

## Deploy Keys
- Allows you attach public keys directly to a repo
- use case:
  - Build servers or CI/CD third-party
  - Single Repo Access
  - Avoid using PAT

## Personal Account Access Tokens (PAT)
- Are on alternative to using passwords for authentication to Github
- Two types of PATS:
  - Classic Tokens
  - Fine-grained personal access tokens
  
# Github APIs
Has two APIs:
- REST API
- GraphQL API

## REST API
- Resource-based
- Differendt endpoints per resource
- Uses GET, POST, PUT, DELETE for operations
- Multiple requests for related data
- Can have over fetching or under-fetching
- Less efficient for complex systems
- Easier due to HTTP methods
- Generally easier to learn
- Server-driven structure
- Often requires API versioning
- Mature, with extensive tools

## GraphQL API
- Single endpoint, query for precise data requests
- Mainly uses POST for all operations
- Single request for complex, related data
- Precise data fetching, no over/under-fetching
- More efficient for complex queries
- More challenging due to POST method
- Steeper but offers powerful features
- Client-driven, highly flexible
- Less need for versioning
- Growing, with unique tools for queries

## Github SDKs
- Octokit are the official SDKs to programmatically interact with the Git REST API
- Github official maintains SDKs for these languages:
  - JavaScript/TypeScript
  - C#/.NET
  - Ruby
  - Terraform

## Github Desktop
- Is stand-alone application to interact with Github repos without the browser or via code
- Accessible only on installed computer
- Manage local copies of repositories
- Simplified interface for commit, pull, push
- Focuses on local repo management
- Simplified experience for basic features
- Limited to local Git tools
- Github Desktop supports:
  - MacOS
  - Windows
  - Linux

## Github Mobile
- You can install on iOS or Android phones to perform redd-only or basic Github repo management tasks
- Can be used for UFA
 
### Github Mobile Notifications

#### Push Notifications 
You set what push notifications you want to receive:
- Direct mentions
- Review Requested
- Assigned
- Deployment Review
- Pull Request Review
- Workflow Runs
Working Hours:
- To only receive push notifications for specific periods of time
Swipe options:
- Save
- Mark as read
- Mark as done
- Unsubscribe

# Types of Github Accounts
There are three of Github accounts:
- Personal
- Organiztional
- Enterprise

## Personal Accounts: 
- These are individual accounts with a username and profile
- They can own resources like repositories and projects and actions taken are attributed to the personal account
- They can use either Github Free or Pro

## Organization Accounts:
- Share accounts where multiple people collaborate
- They can also own resourses like repositories
- Organizations offer different roles with varyiang levels of access and come with security features

## Enterprise Accounts:
- Part of Github Enterprise Cloud and Server, these accounts allow for central management of multiple organizations
- They are geared towards larger setups needing centralized policy and billing management

### Github Free
- Gihub Community Support
- Depedabot alert
- Deployment protection rules for public repositories
- Two-factor authentication enforcement
- 500 MB Github Packages storage
- 120 Github Codespaces core hours per month
- 15 GB Github Codespaces storage per month
- Github Actions Features:
  - 2,000 minutes per month
  - Deployment protection rules for public repositories

### Github Pro
Everything from Github Free and...
- Github Support via email
- 3,000 Github Actions minutes per month
- 2 GB Github Packages storage
- 180 Github Codespaces core hours per month
- 20 GB Github Codespaces storage per month
- Advanced tools and insights in private repositories:
  - Required pull request reviewers
  - Multiple pull request reviewers
  - Protected branches
  - Code owners
  - Auto-linked references
  - Github Pages
- Wikis
- Repositoy insights graphs

### Github Organizations Plans
- Has three plans:
  - Free
  - Teams
  - Enterprise

#### Free
Everything from Github Free and...
- Team access controls for managing groups
- 2,000 Github Actions minutes per month
- 500 MB Github Packages storage

#### Teams
Everything from Github Organizations Free and...
- Github Support via email
- 3,000 Github Actions minutes per month
- 2 GB Github Packages Storage
- Advanced tools and insights in private repositories
- Required pull request reviewers
- Multiple pull request reviewers
- Draft pull requests
- Team pull requests reviewers
- Protected branches
- Code owners
- Scheduled reminders
- Github Pages
- Wikis
- Repository insights graphs
- The option to enable or disable Github Codespaces

### Github Enterprises Deployment Optins
- Include two deployment optins:
  - Github Enterprise Cloud (hosted on Github.com)
  - Github Enterprise Server (self-hosted)

#### Github Enterprise (both Cloud and Server)
Everything from Github Organizations Teams and...
- Github Enterprise Support
- Additional security, compliance and deployment controls
- Authentication with SAML single sign-on
- Access provisioning with SAML or SCIM
- Deployment protection rules with Github Actions for private or internal repositories
- Github Connect
- Option to purchase Github Advanced Security

#### Github Enterprise Cloud (specific features)
- 50,000 Github Actions minutes per month
- 50 GB Github Packages storage
- A service level agreement for 99,9% monthly uptime
- Option to centrally manage policy and billing for multiple Github.com organizations with an enterprise account
- Option to provision and manage the user accounts for your developers, by using Enterprise Managed Users

# Markdown 
- A markup language is a way of formatting and prresenting text data in a different format
- A commom use-case for a markup language is to present data in HTML
- Markdown is markup language that provides a shorthand syntax to format information into HTML
- Markdown is popular due to its easy syntax, and being readable in its raw format
- Markdown files extension are .md and .markdown

## Markdown Basic Syntax
All markdown parsers supports the following markdown syntax:
- Headings: #
- Text formatting : *
- Blockquote: >
- Unordered List: -
- Ordered List: 1.
- Link: [...](...)
- Image: ![alt txt](image)
- Code inline: ``
- Horizontal Rule: ---

## Extended Syntax
- Table
- Fenced Code Blocks
- Footnote
- Task list
- Emoji
- Subscript
- Supersript
- Heading ID
- Definition List
- Strikethrough: ~~
- Highlight: ==

### Text Formatting toolbar
Every comment field on Github contains a text formatting toolbar, which allows you to format your text without learning Github flavowed markdown syntax

### Slash Commands
Slash Commands(within comment boxes) on Github.com provides convenience features such as formatting markdown

## Github Flavowed Markdown (GFM)
- Is the dialect of markdown that is currently supported for user content on Github.com and Github Enterprise
- GFM can render mathematical expressions via latex formatted math
  - $$ or ```math
- GFM will turn raw link automatically into a link 
- GFM provides porwerful functionality:
  - Collapsible sections
  - Embed mathematical expressions
  - Embed diagrams
  - Relative paths or linking to files in the same repo
  - Tasks lists can be converted into issues
  - Extended formatting for tables
  - Shorthands to autolink to issues, pull requests and repos
  - Render code snippets from other codebase via linking
 
### Mermaid
is a markdown inspired tool that renders text into diagrams

### GeoJSON or TopoJSON
Syntax to create interactive maps

### ASCII STL
syntax directly in markdown to create interactive 3D models

### Uploading files
- You can directly upload files by dragginf them into the markdown supported textareas in Github
- Github will host the file with a directory similar to your Git Repo
  - Assume files you upload for public repos are public
- The maximum file size is:
  - 10 MB for images and gifs
  - 10 MB for videos uploaded to a repository owned by a user or organization on a free Github plan
  - 100 MB for videos uploaded to a repository owned by a user or organization on a paid Github plan
  - 25 MB for all others files
- Supported files:
  - PNG
  - GIF
  - JPEG
  - SVG
  - Log files
  - Markdown Files
  - Word
  - Powerpoint
  - Excel
  - Text
  - PDF
  - Zip

 ## Github User Profile Features
 - For personal accounts you can have a public Github User Profile to showcase yourself as a developer
 - User profile include:
   - Profile Picture
   - Bio
   - User Profile Readme
   - Repos
   - Contributions Graph
   - Followers and Followinf
   - Stars
   - Organizations
   - Contribution Activity

## Readme files
- Are markdown files that provided documentation instructional information
- A repo that has a Readme.md or README file in **project´s root** will be rendered on the Github repo page for each access

# Basic Repo Navigation
- Within a Github repo you'll have a navigation bar to the various feature of your Github repo:
  - Code
  - Issues
  - Pull Requests
  - Actions
  - Projects
  - Wiki
  - Security and quality
  - Insights
  - Settings

## Repo Insights
- For Github Repo under the Insights tab you can gain lots of statistical graphs about the repo.
- Not listed as an available feature in the Github free
- Insights contains:
  - Pulse
  - Contibutors
  - Community Standards
  - Commits
  - Code Frequency
  - Dependency Graph
  - Network
  - Forks 

 ### Pulse Contains:
 - pull requests open/close ratio
 - issue open/close ratio
 - Summary of activity
 - Graph of top contributors
 - List of merged pull requests
 - List of issues closed
 - List of issues opened
 - List of unresolved conversations

### Contributors contains:
- Graph of all commits over a time period
- Graph of specific contributors commits over a time period

### Community Standards contains:
- A checklist of recommend community standards and how much a community profile has completed
- this graph will only show for repos that have community profiles
- Community profiles are for open source projects on Github

### Commits contains:
- Number of commits per week for the last 52 weeks (for a year)
- the average number of commits by day of the week for the selected week

### Code frequency contains:
- The amount of additions and deletions of code to report per month

### Dependency graph contains:
- List of dependecies
- List of dependents
- Export Software Bills of Materials (SBOMs)

### Network contains:
- 100 most recently pushed forks
  - you can read the commits to determine the difference of these forks
 
### Forks contains:
- Contains a list of filterable forks

## Issues
tracking tasks, bugs, enchancements, and other actionable items
- often linked to code changes
- can be linked to PRs
- upto 3 issues can be pinned so the appear at the top of the Issue page
- you can apply filters rules to quickly sort through lots of issues, filters contains:
  - Open issues and pull requests
  - Your issues
  - Your pull requests
  - Everything assigned to you
  - Everything mentioning you
  - Advanced search syntax
 
### Issues Templates
- Are markdown templates that are preloaded for new Issues
- They help ensure users creating issues provide all the relevant and expected information
- Issue templates are stored as markdown files in .github/ISSUE_TEMPLATES folder in your repo
- Types of Issue Templates:
  - Bug report
  - Feature request
  - Report a secury vulnerability

### Issue Forms
- Is the evolution of Issues Templates
- You use a YAML formatted file to create Issue forms for stricter entry of issue information

## Discussions  
Facilitating conversations and Q&As about a wide range of topics related to the project
- categorized by topics
- Can be "converted" to issue (create a issue with a soft link to the issue)
- not directly linked to code changes 

## Pull Requests
Proposing, reviewing, and merging code changes into the codebase
- Benefits of a Pull Request:
  - Colaborative Review
  - Change tracking
  - Automated Testing
  - Controlled Integration
  - Open Source Friendly
- Directly linked to code changes
- can be linked to issue
- A PR is not a feature of git, but a workflow

### Creating a Pull Requests
- We can use the Github CLI to create a PR
- In the Github repo use navigation to Pull Requests and we create a new PR
- we set the:
  - Base
  - Head

### Linked Activiy within a PR
- You can link issues to PR so that the state of the PR will automatically close the issue
- You can link a PR to an issue by using a supported keyword in the pull requests description or in a commit message
- The PR must be on the default branch

#### Base and Compare
Determines the direction of the merge for a pull requests
- Base: is who you want to merge into, this is usually the main branch
- Compare: is what will be merged into Base, compare is choosing a Head ref
  - this is usually a bug or feature branch
  - you can also compare across forks, this is how a fork stays up to date

### Draft Pull Requests
A Draft Pull Requests on Github is a feature that allows you to open a pull request but mark it as a work-in-progress(WIP)
- Draft pull requests **cannot be merged**
- code owners are not automatically requested to review draft pull requests
- is a feature only for Github Organizations Teams
- use case for draft pull requests:
  - Indicating WIP
  - Preventing premature merging
  - Facilitating Early Feedback and collaboration
  - Continuos Integration testing
  - Transitioning to a Ready State
  - Organizing work and priorities  
  
### PR Status
- Open
- Draft
- Closed
- Merged
- Changes requested
- Review Required
- Approved
- Conflict
- Ready for Review

### PR Options
When merging a PR there are a few options:
- Create a merge commit: all commits will be added
- Squash and merge: 1 commit will be added
- Rebase and merge 1 commit will be added and rebased

### PR Templates
- Are similar to issue templates
- They will populate the pull request textarea with the specified template
- You can create multiple PR templates in a folder called .github/PULL_REQUEST_TEMPLATE

### Commenting in Pull Requests
- When you comment you are submitting a review to be considered before a Pull Request is being accepted
- If you are not the author, but also a designated reviewer you can **request changes** or mark the PR as **approved** so it can be considered for merging
- Under **files changed** you can also apply a review on a very specific line of code
- 
### Required Reviewers
PR can have multiple required reviewers who must write a review that approves the changes

### Codereviews with CODEOWNERS file
- CODEOWNERS Github repo specific file to define individuals or teams that are responsible for specific code in a repository
- CODEOWNERS files uses a similar syntax to .gitignore
- When a PR is opened that modifies any files matching a pattern in the CODEOWNERS file, Github automatically requests a review from the specified code owners

### Creating a new Repo
- When you create a repo you choose a owner:
  - Personal account
  - An organization that you belong to
- Choose an available github repo name
- repo can either be public or private
- you can quickly add a:
  - Readme file
  - .gitignore file
  - License file
- Github CLI can be used ti create a Github repo

### Adding files to a repo
- Within the Github UI:
  - multiple text and binary files can be uploaded
  - new single file can be created
- You can also create nested folders by typing a forward slash in the filename

### Starring repos
- Similar to bookmarking, it's a way to mark a repository as interesting on to keep track of it for reference
- Stars are public and can be seen by everyone, often used as a measure of a project´s popularity

### Whating repos
- Whating a repo allows you to stay informed about activies ocurring within a repo

### Features previews
- Allows you to enable or disable features that are in beta in your personals account

## Tags
- Tagging is used to capture a point in history to marked version release of your codebase
- CI/CD pipelines may be configured to deploy on the presence of a new tag on production branch
- common git tag commands:
```gh
git tag 1.0.0
git push --tags
git checkout 1.0.0
git tag -d 1.0.0
git push --delete origin [tag-name]
```
## Github Releases
Allows you to create releases with release notes and linked assets such as zip source or binaries for specific platforms

## Github Packages
- Is a platform for hosting and managing packages, including containers and other dependecies
- Supporrted package registry:
  - JavaScript
  - Ruby
  - Java
  - .NET
  - Docker
# Github Discussions
Is community Communication tool for your public or private Github repos
- has:
  - Threaded Conversations
  - Categorization
  - Community Interaction
  - Markdown Support
  - Pin Discussions
  - Conversation Polls
  - Discussion Volting
  - Conversion to issues
  - Notifications
  - Seachable and linkable
  - Github Integration
## Discuussion Options
- When someone creates a discussion they need to choose a category
- Github provides some Categories but Github repo owners can create their own
- When you create a new category you will choose a Discussion Format:
  - Open-ended discussion
  - Question/Answer
  - Annoucement
  - Poll

### Marking answers in a discussion
For a Q&A discussion you can mark an answer as the recomended answer regardless of upvotes to help direct which question you think is the most credible

### Pining Discussions
puts discussions fixed at the top of the community page

## Notification Configuration Options
In your account settings you have a Notification tab to configure notifications options
### Notificaiton filters Options
- filter notifications using a filtes syntax
- predefined saved filters
- you can create more saved filters using filter syntax
- you can group notification
  - Threads by repo or by date 
### Mentions in threads
Is when someone using a @ followed by your username
### Notification Inbox
- Provides a chronological list of notifications threads
- allows you to keep on top of all subscribed activities with associated repo
### Notification Watching
- you can wath repos in order to get notified of activities
- your own repos you already set as watching
### Notifications Subscriptions
- Allow you to follow activities for a specific PR or issue
- you can see all your subscriptions under Notifications

# Github Gists
- Provide a single way to share code snippets with others
- Every gist is a Git repository, which means that it can be forked and cloned
- Gists can be public or secret
- you can pin Gists to your profile for others
- allow other users to comment
- allow you to easly navigation revisions
## Gists Public
- are searchable
- show up in Discover
- cannot be changed to be private
## Gists Secret
- are not searchable and do not show up in discover
- are not private
  - you can share the URL with friends
- can be changed to be public

### Create a Gists
- Name it
- Provides the filename with extension
- the file extension will allow the file to apply syntax highlighting
- provide code
- attach associate files to the gist
- set it as either secret or private

# Github Wiki Pages
- A wiki is collaborative way to quickly create documentation with multiple nested pages
- a wiki woild serve as a knowledge base for your repo or organization
## Managing Github Wiki Pages
- When you create a page you can use various markup languages
- to lin to other pages you provide the Github wiki pages table as the link

## Wiki pages visibility
- If you create a wiki in a public repository, the wiki is available to the public
- If you create a wiki in a private repository, only people with access to the repository can access the wiki

# Gihub Pages
- Allows you to directly host a static website via a Github repository
- You need to create a public repo
- You simply add HTML files and assets to your repo
- Jerkyll is static site generator which allows you to build complex static sites or blogs with ease

# Github Actions
- Is a CI/CD pipeline directly integrated with your Github repository
- Github actions files are defined as YAML files located in the .github/workflow folder in your repo
- Multiples workflows in repo triggered by different events
- When you run Github Actions you'll get a history of workflow runs where it will indicate if its was success a failure, and how long it took to run
- Github Actions allows you to automate:
  - Running test suites
  - Building images
  - Compiling static sites
  - Deploying code servers
  - and more...
## Types of Github Actions
- Event Triggers causes a Github Action to run
- The **on** atribute specifies the **event trigger** to be used
- Examples of common Github Actions that could be triggered:
  - Pushes
  - Pull Requests
  - Issues
  - Releases
  - Scheduled Events
  - Manual triggers
- Remenber:
  - on
  - jobs
  - steps
# Github Copilot
Is AI developer tool that can be used with multiple IDEs via an extension
- code completion
- chat in IDE and mobile
- CLI assistance
- code referencing
- Public code filter
- IP indemnity
## Github Copilot Individuals
- $10 USD per month or $100 USD per year
- personal accounts
- telemetry
- blocks suggesstions matching public code
- plugs right into you editor
- offers multi-line function suggestions

## Github Copilot Bussines
- $19 USD per user per month
- Organization or Enterprise accounts
- Everithing in individuals, less telemetry
- organizations-wide policy management
- exclude specified files
- Audit logs
- HTTP proxy support via custom certificates
### Setting up Copilot
1. Install the Github Copilot extension
2. Chose trust Workspace
3. Sign in to Github
### Using Copilot
- Copilot is best used when you know or set hotkeys to perform suggestions
- you to have Copilot Chat feature enabled in your personal account or for your organization

# Github Codespaces
- Is Cloud Developer Environment(CDE) integrated with your Github repo
- A codespace runs:
  - In Ubuntu Linux docker container
  - on a virtual machine
  - hosted and managed by Github
- your codebase will be cloned into/workspaces
- you can interact with your codespace via:
  - Command Line
    - SSH via Github CLI
  - Code editors
    - VS Code Browser
    - VS Code Desktop
    - Jetbrains IDE
- when you create a new codesapce you choose:
  - the repo
  - the branch
  - the region
  - machine type
- the region you can choose:
  - US East
  - US West
  - Europe West
  - Southeast Asia
  - Australias
- the capacity of your environment is based on the virtual machine type you choose:
  - 2-core
  - 4-core
  - 8-core
  - 16-core
- there is a limit of concurrent codespaces allowed to run. If you hit the limit you may need to stop other codespaces first
## Codespaces Lifecycle
- Create or reopen an existing one
- running
- rebuild
- Timeouts
- Stops
- Saving and auto save
- Deleting

## Renaming Codespaces
- when you create a codespace it's assigned an auto-generated display name.
- you can rename the auto-generated name in the case you have multiple codespaces to easily identify

### VS Code
- Github Codespaces should persist your VS Code settings
- Github Codespaces should persist your VS Code extensions
- Github Codespaces should persist your VS Code theme
