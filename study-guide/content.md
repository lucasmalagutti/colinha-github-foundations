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
## Organization Teams Tab
- An organization can group organization members in teams
- Teams can be public or private
- Teams can be assigned to projects and issues
- Request reviews from teams
- Teams can be mentioned in discussions, issues, and pull requests
- Control team access to repositories
- New members can be added to teams, instantly giving them access to all relevant repositories and discussions
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
 
 ### Milestones
 - Allow you to group multiple issues into an end goal which show completion towars the goal for each closed issued
 - you associate issues to Milestones
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
## Github Projects
- Is a planning and tracking tool when on working on Github Repo
- new, more dynamic interfaces with tables, boards and views
- Highly customizable with different views and fields
- Supports automated workflows and field updates
- Enchanced reporting features and insights
- Deeper integration with Github issues and pull requests
- A project has an adaptable view that can be changed at anytime between:
  - Spreedshet(Table)
  - Taskboard(Board)
  - Roadmap
- Projects directly integrate with issues and Pull requests
- Projects have built-in workflows to automate common actions
- A github project is composed of multiple views
- Each view's layout can be changed at anytime
- For your layouts you can configure your data based on multiple options
### Projects Classic
- tradicional board view similar to Trello
- limited customization options
- basic automation capabilities
- basic reporting and tracking
- basic integration with Github repositories
### Project Workflow
- Github built-in Project Workflows allows you to automate what happens based on specific events
- Built-in workflows:
  - item added to project
  - item reopened
  - item closed
  - code changes requested
  - code review approved
  - pull request merged
  - auto-archive items
  - auto-add to project
- for more advanced automation of Github Projects you can use Github Actions
### Project Insights
- lets you create charts about your Github Project
- has two:
  - **Current Changes:**
    - how many items are assigned to each individuals
  - **Historical Changes:**
    - track changes to the state off your project items 
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
### Managing Saved Replies
When commenting on an issue or pull request, you can add saved reply that you've already set up
### Assigning Issues and Pull Requests
You can assign issues and pull requests to specific users
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
- Free montly quota, storage and core hours per month, machine type changes cost
- Takes a few minutes to startup, does load devcontainer.json
- Dedicated attached VM
- Run and delay your code and apps
- Terminal access
- Most extensions for them VS Code Marketplace
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

## Retention Period and Timeout Configuration
- Under Github Settings > Codespaces you can change the **timeout** and **retention period**
- How long should codespaces wait to stop a codespace when their has been no activity:
  - Min: 5 minutes
  - Max: 240 minutes (4h)
  - Default: 30 minutes
- How many days should pass until inactive codespaces are automatically deleted:
  - Min: 0 days
  - Max: 30 days
  - Default: 30 days
### Codespaces Sync Settings
- You can have codespaces able to pull from VS Code Settings Sync service
- VS Code settings sync lets you share your VS Code configs such as settings, keybindings, and installed extensions across your machines
### Installing dotfiles
- you can configure Github Codespaces to use dotfiles from a specific repository that will be used for all future codespaces you start
- When you create a new codespace with this feature, Github does two things:
  1. clones you selected dotfiles repository to the codespace environment
  2. looks for one of the following files to set up the environment
     - install
     - setup
     - bootstrap
     - and more...
### Codespaces Deep Links
Is an easy to way to generate a shareable link that will launch a codespace for a specific repo

### Codespaces Secrets
- Under Github Settings > Codespaces tou can set Github secrets
- Secrets allows you to set sensitive environment variables that will be loaded into your codespace this avoids hardcoding secrets, passwords or sensitive values into your codebase

## Dev Container Configuration
- VS Code dev container allows you to configure your docker container via json file
- devcontainer.json file is expected in the root of you project
- you can provide remote image from a repo
- you can build your own image by including the Dockerfile with your project
- to custom configure program generally you will install these via your custom Dockerfile
- features allows you to quickly install programs on top of a common base image
- tou could use the ```postCreateCommand``` to install a bouch a programs
- Command flags and their values we want to pass to when ```docker run``` command
- Mounts allows you to map files and folders to your container
  - Bined mount a local directory
  - Mount a Docker volume for persistent storage
  - Mount the Docker Socket
  - Mount a specific file
  - Mount a Host Directory as readonly 
### VS Code
- Github Codespaces should persist your VS Code settings
- Github Codespaces should persist your VS Code extensions
- Github Codespaces should persist your VS Code theme
### Changing Shell
- Github Codespaces VS Code browser defualt devcontainer.json image come with:
  - Bash (default)
  - zsh
  - fish
- If you build or provide an image to devcontainer.json with other shells installed you can define and provide the path to that shell for use
- You can configure the settings in the VS Code to change defaults based on OS.

# Github.dev
- Free
- Available to everyone on Github
- Instantly lauches, no devcontainer.json configuration
- there is no attached compute
- you can't run code or apps
- no terminal
- limited subset of extensions
- Is a VS Code browser that instantly loads that has no attached compute
- Two ways you can open Github repo in Github.dev:
  1. Press the period (.) hotkey when you have your Github repo page opened
  2. place your Github path after the url:
     - github.dev/<user/org>/<repo-name>
- Github.dev is intended for quickly changes to file and commiting code in an IDE experience

# Open Source
- Open source is sorce code made freely available for possible modification and redistribution
- Public, global community
- Open to anyone (devs, users etc.)
- Share and collaborate on projects globally
- Public available and visible
- Usually governed by open source licenses and community rules
- Open source benefits include:
  - Encorages global collaboration
  - Speeds up innovation
  - Offers adaptability and customization
  - Reduces software costs
  - Enchances learning for developers
  - Typically high-quality and reliable
  - Provides Transparency for trust and security
- Open source softwares has often have free community versions which makes it easy for personal developers or small organizations to quickly adopt techonology
- Open Source Iniatiative (OSI) is a non-profit organization is the steward of the Open Source definition, the set of rules that define open source software
- The OSI maintains a list of open source licensing documents for all different  use-cases which are readability available for project owners to adopt
- top five most popular open source licenses:
  1. MIT License
  2. GNV General Public License(GPL)
  3. Apache License 2.0
  4. GNV Lesser General Public License(LGPL)
  5. BSD License
## Github an open source projects
- when create a new repo Github mates it easy to quickly add a selected open source license to your repo
- they will display this on the Github repo page
- The file in the repo will be listed as either:
  - license.md
  - LICENSE
  - LICENSE.md
## Open Source discovery
- Github search makes it easy to find public repos based on open source license
- In explore:
  - Github topics allows you to find repos for specific categories
  - Github Trending: shows you most popular repos
## Inner Source
- InnerSource is organization and development best practives of non-opne-source and/or proprietary software
- is not a strict guideline bus a loose strategy to establish an open source like culture within organizations
- limited to company employees
- improve collaboration and efficient internally
- Code and discussions often private to the organization
- Dictated by internal policies and culture

## Github Sponsors
- Allows Github users to collect donations for their Github hosted own source project
- Sponsorship paymenys are facilitated two ways:
  1. payment through Github
  2. payment through Patreon
- To receive sponsorship through Github you'll need to get accepted into Github Sponsors
- Github makes it easy to locate people who maintains your dependencies so you can support open source contributors

 ### Following Organizations 
 - On a Github Organizations public profile you can choose to follow them to notifications of their public activity on your personal dashboard
 - This activity includes:
   - new discussions
   - sponsorships
   - repositories
## Github Marketplace
- Are apps that integrate with your Github repos to provide additional functionality
- Apps can be free or paid
# Forking
- Forking repos allows you to create a copy of a repo
- allows you to:
  - Take a open source or source available repo and go your own way
  - Quickly apply bugs and patch fixes
  - A separate repo to work on community contributions
- you can crete cross-repo pull requests to get accepted in the original repo
- using Network Graph under Repo Insights you can often find community solutions to bugs or missing features

## Discoverable repos 
- Github Repos can be set as public, making repos easily searchable on Github and via search engines
- Public repos serve a community purpose for knowledge sharing, educational resources and open source projects
- Github provides a robust search that lets us not only repos names but the contents of their repos
- Github also has several advanced search options
- Search syntax:
  - Github global search box has a search syntax to help quickly apply advanced search options
## Labels
- Github labels are used to categorize issues, pull requests, and discussions
- you can apply multiple labels to a labels item
- you can manage your labels or create new
- Creating a label as simple as providing a:
  - name
  - descriptions
  - colour
- Github CLI provides commands for labels
# Security Account with 2FA
- 2-Factor Authentication(2FA) is when you use a device (phone) to enter a code as an extra security precaution when signing-in or performing sensitive actions
- Choose your prefered UFA:
  - Github mobile
  - SMS/ Text message
  - Authentication app
- Hardwares devices like Yubikey
- Recovery codes are long secret codes you need to print and store someone safe in case you get locked out
## Access Permissions - Personal Accounts
- has two permission levels:
  - Repository owner
  - Collaborators
### Repository owner actions
has full control of the repository 
### Collaborators actions
can pull the contents of the repository and push changes to the repository

# EMUs
- Enterprise Managed Users (EMUs) allows you to manage the lifecycle and authentication of your users on Github from a external identity management system, or IdP
- Github partners with some developers of identity management system to provide a "paved-path" integration with EMUs
- These IdPs mostly provide authentication using SAML
- Microsoft Entra ID (aka Azure AD) alos offers OIDC for authentication
- The IdP applications provision users with system for cross-domain Identity Management (SCIM)
- Partner IdP:
  - Microsoft Entra ID:
    - SAML
    - OCID
    - SCIM
  - Okta and PingFederate:
    - SAML
    - SCIM
## **Security Scanner**
- Dependabot
- Code Scanning
- Secret Scanning
## Repo permission levels
- when you add a collaborator you can choose from predefined roles with different level of access
- Read:
  - View and clone the repo
  - Open and comment on issues and PRs
  - Download releases
- Triage:
  - manage issues and pull requests without write access
  - label and assign issues and pull requests
  - close and reopen issues and pull requests
- Maintain:
  - Push to the repo
  - Manages issues, PRs, labels, and project
  - create and publish releases
  - configure repository settings for non-sensitive fields
- Admin:
  - Full Control over the repo
  - push to, delete, or archive the repo
  - change repo settings, including sensitive fields like security or billing
  - manage collaborators and their permissions
  - access to all functionalities provided in the maintain role
## Branch Protection Rules
- are used to enforce certain workflows or requirements before changes can be merged into a branch
- protect matching branches rules:
  - Require a pull request before merging
  - require a status checks to pass before merging
  - require a conversation resolution before merging
  - require a signed commits
  - require a linear history
  - require a deployments to succeed before merging
  - lock branch
  - do not allow by passing the above settings
- Rules applied to everyone including administrators
  - allow force pushes
  - allow deletions
## Security Tab features and options
The security tab will present a repo security checklist of security options to configure
- Security policy
- Security advisories
- Private Vulnerability Reporting
- Dependabot alerts
- Code scanning alerts
- Secret scanning alerts

## Github Connect
- Enchances Github Enterprise Servers (GHES) by allowing your GHES instance access some of Github cloud only offerings
- you can individually enable these features:
  - Automatic user license sync
  - Dependabot
  - Github Actions
  - Server Statistics
  - Unified search
  - Unified contributions

 ## Github Internal Repos
 - Github Enterprise Cloud accounts have a third special Github Repo type called Internal
 - All enterprise members have read permissions to the internal repository
 - Internal repositories are not visible to people outside of the enterprise, including outside collaborators on organization repositories
 - Unless your enterprise uses Enterprise Managed Users (EMUs), members of the enterprise can fork any internal repo owned by a organization in the enterprise
 - Internal repositories are the default setting for all new repositories created in an organization owned by a enterprise account
## Github Advanced Security
- Github makes extra security features available to customers under a Github Advanced Security (GHAS) license
- is available for enterprise accounts on:
  - Github Enterprise Cloud
  - Github Enterprise Server
  - And some features of for public repositories on Github.com
- Provides the following additional features:
  - Code scanning
  - Secret scanning
  - Dependancy review
## SAML and SCIM
- SAML and SCIM is available for both Github Enterprise Cloud and Github Enterprise Server
- Security Assertion Markup Language (SAML) is open standard for exchanging authentication and authorization between an identity provider and a service provider
- An important use case for SAML is Single Sign-on via web browser
- System for Cross-domain identity Management (SCIM) is an open standard for automating the exchange of user identity information across different identity management systems
- A key use case for SCIM is to enable and automated user provisioning and deprovisioning, often integrated with enterprise identity services
- SAML is about securely transmitting user authentication and authorization data for single sign-on purposes
- SCIM is about managing user identites across different systems to simplify account maintenance and provisioning
- They can complement each other in an ecosystem where you need both federated identity for authentication and a standardized way to manage user accounts across various systems
