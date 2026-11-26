# GitHub Foundations - Practice Questions

1. What is the primary difference between Git and GitHub?
    Select only one answer.
    - Git is a cloud-based hosting service, while GitHub is a local command-line tool.
    - Git is a distributed version control system, while GitHub is a cloud-hosted platform built around Git.
    - Git is used exclusively for private repositories, while GitHub is only for open-source projects.
    - Git requires an active internet connection for every action, whereas GitHub works entirely offline.

2. Which type of Version Control System (VCS) allows every user to have a complete local copy of the entire repository and its history?
    Select only one answer.
    - Centralized Version Control System (CVCS)
    - Local Version Control System (LVCS)
    - Distributed Version Control System (DVCS)
    - Linear Version Control System (LVCS)

3. Which term best describes GitHub's model of providing version control and collaboration tools over the internet?
    Select only one answer.
    - Infrastructure as a Service (IaaS)
    - Version Control as a Service (VCaaS)
    - Database as a Service (DBaaS)
    - Function as a Service (FaaS)

4. Which Git command initializes a new, empty Git repository in your current local directory?
    Select only one answer.
    - git start
    - git init
    - git create
    - git new

5. What is the purpose of the `git clone` command?
    Select only one answer.
    - To create a new branch from the current commit.
    - To download a full copy of an existing remote repository to your local machine.
    - To merge two local branches together.
    - To upload local commits to a remote server.

6. Which command moves modified or newly created files from the working directory to the staging area?
    Select only one answer.
    - git commit
    - git push
    - git add
    - git status

7. How can you view the current state of your working directory and staging area, including tracked and untracked files?
    Select only one answer.
    - git log
    - git diff
    - git status
    - git show

8. Which command records staged changes permanently into the local repository's commit history?
    Select only one answer.
    - git push
    - git commit
    - git save
    - git stage

9. What does the `git push` command do?
    Select only one answer.
    - Downloads new commits from a remote repository without merging them.
    - Sends committed changes from a local branch to a remote repository.
    - Moves files from the working directory to the staging area.
    - Deletes a remote branch permanently.

10. Which command fetches changes from a remote repository and immediately integrates them into your current local branch?
    Select only one answer.
    - git fetch
    - git clone
    - git pull
    - git remote

11. Which Git command allows you to inspect the chronological commit history of a repository?
    Select only one answer.
    - git history
    - git status
    - git log
    - git branch

12. What is the primary function of the `git branch` command?
    Select only one answer.
    - To switch between different remote URLs.
    - To list, create, or delete branches in a repository.
    - To revert a repository back to its initial commit.
    - To compress commit history into a single patch file.

13. Which command is used to manage the set of tracked remote repositories (such as `origin`)?
    Select only one answer.
    - git server
    - git origin
    - git remote
    - git link

14. What does the `git merge` command accomplish?
    Select only one answer.
    - It temporarily saves uncommitted changes in a clean working directory.
    - It combines the commit history of one branch into another active branch.
    - It removes untracked files from the working directory.
    - It creates a duplicate repository on GitHub.

15. When should you use the `git stash` command?
    Select only one answer.
    - When you want to permanently delete all uncommitted local changes.
    - When you need to temporarily shelve uncommitted changes so you can switch branches cleanly.
    - When you are ready to publish a release tag to GitHub.
    - When you want to rename your local repository folder.

16. Which Git command moves staged changes back to the unstaged working directory?
    Select only one answer.
    - git reset
    - git clean
    - git stash pop
    - git rm

17. Why would a developer configure an SSH key with their GitHub account?
    Select only one answer.
    - To increase the maximum file upload limit in GitHub Issues.
    - To authenticate securely with GitHub over Git without entering a username and password on every operation.
    - To enable two-factor authentication via SMS.
    - To automatically deploy GitHub Pages sites.

18. Which step is part of the standard GitHub Flow workflow?
    Select only one answer.
    - Developing all new features directly on the `main` branch without pull requests.
    - Creating a dedicated feature branch from `main`, committing changes, opening a Pull Request, and merging after review.
    - Creating separate release, hotfix, and develop branches for every minor typo fix.
    - Locking the repository so only one developer can clone it at a time.

19. In GitHub Flow, why is it important to keep the `main` branch deployable at all times?
    Select only one answer.
    - Because GitHub automatically deletes branches that are not deployed within 24 hours.
    - Because `main` serves as the single source of truth from which new branches are created and production releases are made.
    - Because Pull Requests cannot be opened if `main` has more than ten commits.
    - Because GitHub Actions only runs on branches named `production`.

20. What are the two primary API types offered by GitHub for programmatic integration?
    Select only one answer.
    - SOAP API and XML-RPC API
    - REST API and GraphQL API
    - gRPC API and WebSocket API
    - ODBC API and JDBC API

21. What is the key advantage of using GitHub's GraphQL API over the REST API?
    Select only one answer.
    - It does not require any authentication token for private repositories.
    - It allows clients to request the exact data structure they need in a single request, avoiding over-fetching or under-fetching.
    - It is the only API that supports webhooks.
    - It automatically converts Markdown files into PDF documents.

22. What is Octokit?
    Select only one answer.
    - A GitHub-hosted runner for macOS builds.
    - The official suite of client libraries and SDKs provided by GitHub to interact with its APIs in multiple programming languages.
    - A command-line tool used exclusively for resolving binary merge conflicts.
    - A security scanner that detects leaked API keys in public gists.

23. Which official GitHub application provides a visual graphical user interface (GUI) for performing common Git operations on Windows and macOS?
    Select only one answer.
    - GitHub Codespaces
    - GitHub Desktop
    - GitHub CLI
    - GitHub Copilot

24. Which tasks can you perform using GitHub Mobile?
    Select only one answer.
    - Run heavy Docker containers locally on your phone.
    - Triage notifications, review and merge Pull Requests, and manage Issues on the go.
    - Configure enterprise SAML single sign-on servers.
    - Host self-hosted GitHub Actions runners directly on iOS.

25. Which GitHub account type is designed for an individual user's personal projects and contributions?
    Select only one answer.
    - Organization account
    - Enterprise account
    - Personal account
    - Team account

26. What is the primary purpose of a GitHub Organization account?
    Select only one answer.
    - To serve as an individual's personal portfolio and contribution graph.
    - To provide shared ownership of repositories where businesses or open-source communities can collaborate with granular team permissions.
    - To act as a billing-only wrapper that cannot own any repositories.
    - To store personal gists privately.

27. Which GitHub account type enables centralized management, billing, and security policies across multiple Organizations?
    Select only one answer.
    - Personal Pro account
    - Organization account
    - Enterprise account
    - Collaborator account

28. Which GitHub plan provides unlimited public and private repositories for individual developers at no cost?
    Select only one answer.
    - GitHub Free
    - GitHub Pro
    - GitHub Team
    - GitHub Enterprise

29. Which feature is included when upgrading from GitHub Free to GitHub Pro for a personal account?
    Select only one answer.
    - Unlimited self-hosted runners with free hardware provided by GitHub.
    - Advanced insights, GitHub Pages on private repositories, and increased GitHub Actions minutes and Packages storage.
    - Enterprise Managed Users (EMU).
    - Dedicated 24/7 phone support with a 15-minute SLA.

30. Which paid plan is tailored specifically for collaborative teams working inside a GitHub Organization?
    Select only one answer.
    - GitHub Pro
    - GitHub Team
    - GitHub Student Developer Pack
    - GitHub Free for Individuals

31. What does GitHub Enterprise offer that is not available on GitHub Free or GitHub Team?
    Select only one answer.
    - Public repositories and Pull Requests.
    - Enterprise-grade security, SAML single sign-on (SSO), advanced auditing, and options for Enterprise Cloud or Enterprise Server.
    - Basic Markdown rendering in README files.
    - Ability to fork public repositories.

32. What is GitHub Flavored Markdown (GFM)?
    Select only one answer.
    - A proprietary programming language used to write GitHub Actions workflows.
    - GitHub's extension of standard Markdown that adds features like task lists, tables, strikethrough, and automatic URL linking.
    - A CSS framework used to style GitHub Pages websites.
    - A tool for converting Jupyter Notebooks into plain text.

33. How do you create an interactive task list inside a GitHub Issue or Pull Request using GitHub Flavored Markdown?
    Select only one answer.
    - Using `[x]` and `[ ]` preceded by a list marker such as `- [ ] Task`.
    - Using `<checkbox>` HTML tags.
    - Wrapping text in double curly braces `{{Task}}`.
    - Using `#todo` before each line.

34. Which syntax is supported natively in GitHub Markdown blocks to render flowcharts, sequence diagrams, and Gantt charts?
    Select only one answer.
    - PlantUML code blocks
    - Mermaid code blocks (```` ```mermaid ````)
    - LaTeX TikZ blocks
    - SVG inline scripts

35. Which geographic data format can GitHub automatically render as an interactive map when committed as a file or included in a Markdown block?
    Select only one answer.
    - Shapefile (`.shp`)
    - GeoJSON (`.geojson` / `.topojson`)
    - KML (`.kml`)
    - GPX (`.gpx`)

36. Which 3D model file format does GitHub natively render with an interactive 3D viewer directly in the browser?
    Select only one answer.
    - `.obj`
    - `.blend`
    - `.stl` (ASCII or binary STL)
    - `.fbx`

37. What happens when you drag and drop an image or supported file into a GitHub Issue or Pull Request comment box?
    Select only one answer.
    - The file is committed directly to the `main` branch of the repository.
    - GitHub uploads the asset to its CDN and automatically inserts the corresponding Markdown link into the comment.
    - The file is emailed to all repository watchers.
    - GitHub rejects the upload unless the file is smaller than 10 KB.

38. Where does GitHub automatically display the rendered content of a `README.md` file?
    Select only one answer.
    - Only inside the repository's Wiki tab.
    - On the main front page of the repository below the list of files and directories.
    - Inside the Settings tab under General.
    - Only when a user downloads the repository as a ZIP archive.

39. What is a best practice for writing an effective `README.md` file?
    Select only one answer.
    - Include the entire source code of the application inside the README.
    - Clearly explain what the project does, why it is useful, how to install/use it, and how others can contribute.
    - Avoid using headings or code blocks so the file stays plain text.
    - Update the README only after the project is archived.

40. Which repository tab provides an activity overview showing recent Pull Requests, Issues, and active contributors over a selected time period?
    Select only one answer.
    - Insights > Pulse
    - Security > Advisories
    - Actions > Workflows
    - Settings > Collaborators

41. Where in a repository can you view a ranked graph of who has authored the most commits over time?
    Select only one answer.
    - Issues > Milestones
    - Insights > Contributors
    - Pull Requests > Checks
    - Code > Branches

42. What is the purpose of the Dependency Graph in a GitHub repository?
    Select only one answer.
    - To visualize the hierarchy of Git branches and tags.
    - To identify the manifest and lockfiles in a repository and list all direct and transitive packages the project depends on.
    - To track how many hours each developer spent coding.
    - To display the geographic locations of repository visitors.

43. Which section under the Insights tab checks whether a repository includes recommended health files like a `README`, `LICENSE`, `CONTRIBUTING`, and `CODE_OF_CONDUCT`?
    Select only one answer.
    - Insights > Traffic
    - Insights > Community Standards
    - Insights > Forks
    - Insights > Network

44. What is a "fork" in GitHub?
    Select only one answer.
    - A local Git branch that has not been pushed to any remote.
    - A personal copy of another user's or organization's repository under your own GitHub account.
    - A deleted commit that can only be recovered via `git reflog`.
    - A webhook event triggered when an Issue is closed.

45. How do you propose changes from your forked repository back to the original ("upstream") repository?
    Select only one answer.
    - By running `git push upstream main` directly without permissions.
    - By opening a cross-repository Pull Request from your fork's branch to the upstream repository's branch.
    - By emailing a `.patch` file to GitHub Support.
    - By converting your fork into a GitHub Gist.

46. What is the purpose of a `.gitignore` file in a repository?
    Select only one answer.
    - To list users who are blocked from commenting on Issues.
    - To specify intentionally untracked files and directories (such as build artifacts or `.env` files) that Git should ignore.
    - To prevent GitHub Actions from running on specific branches.
    - To hide public repositories from search engines.

47. What is a GitHub Gist?
    Select only one answer.
    - A full enterprise CI/CD pipeline orchestrator.
    - A simple, lightweight way to share code snippets, notes, or single files, backed by its own Git repository.
    - A tool for managing organization-wide SAML authentication.
    - A replacement for GitHub Projects boards.

48. Which GitHub feature allows you to host static websites directly from a repository?
    Select only one answer.
    - GitHub Packages
    - GitHub Pages
    - GitHub Codespaces
    - GitHub Sponsors

49. What is the difference between a repository's **Watch** and **Star** features?
    Select only one answer.
    - Starring subscribes you to all issue and PR notifications, while Watching bookmarks the repo.
    - Watching subscribes you to notifications about repository activity, while Starring bookmarks the repository and shows appreciation.
    - Watching gives you write access to the repository, while Starring gives you admin access.
    - There is no difference; both perform the exact same action.

50. Which file in a repository defines the legal terms under which others can use, modify, and distribute the code?
    Select only one answer.
    - `CONTRIBUTING.md`
    - `SECURITY.md`
    - `LICENSE` (or `LICENSE.md`)
    - `CODEOWNERS`

51. What is the function of a `CODEOWNERS` file in a repository?
    Select only one answer.
    - It transfers legal billing ownership of the repository to another user.
    - It automatically requests reviews from designated individuals or teams when Pull Requests modify specific files or directories.
    - It lists all third-party open-source licenses used in the project.
    - It locks files so no one can edit them locally.

52. In GitHub Issues, what is the purpose of **Labels**?
    Select only one answer.
    - To assign write permissions to external contributors.
    - To categorize, filter, and prioritize issues and pull requests (e.g., `bug`, `enhancement`, `documentation`).
    - To trigger automated Docker builds on every commit.
    - To archive old repositories automatically.

53. What is a **Milestone** in GitHub?
    Select only one answer.
    - A tag created automatically when a repository reaches 1,000 stars.
    - A way to group related Issues and Pull Requests together to track progress toward a specific goal, release, or sprint.
    - A required approval from an Organization owner.
    - A backup snapshot of a repository's Wiki.

54. Which syntax in a Pull Request description automatically closes an Issue (e.g., Issue #42) when the Pull Request is merged into the default branch?
    Select only one answer.
    - `See #42`
    - `Fixes #42` (or `Closes #42`)
    - `Mentions #42`
    - `Links #42`

55. What is a **Draft Pull Request**?
    Select only one answer.
    - A Pull Request that has already been merged and locked.
    - A Pull Request that signals work is still in progress and cannot be merged until it is marked as "Ready for review."
    - A Pull Request created automatically by Dependabot.
    - A Pull Request that is visible only to repository administrators.

56. What is the difference between **Squash and merge** and a standard **Create a merge commit** when merging a Pull Request?
    Select only one answer.
    - Squash and merge deletes the target branch, whereas a merge commit deletes the source branch.
    - Squash and merge combines all commits from the Pull Request branch into a single commit on the base branch.
    - Squash and merge can only be used on private repositories.
    - Create a merge commit rewrites commit timestamps to the current time, whereas Squash and merge preserves all individual commits.

57. Which GitHub feature provides cloud-hosted, instant, pre-configured development environments accessible directly from your browser or VS Code?
    Select only one answer.
    - GitHub Pages
    - GitHub Codespaces
    - GitHub Packages
    - GitHub Discussions

58. What is **GitHub Actions** primarily used for?
    Select only one answer.
    - Hosting static HTML documentation websites.
    - Automating software development workflows, including CI/CD pipelines, triggered by GitHub events.
    - Managing personal billing invoices.
    - Editing 3D STL models in the browser.

59. What is **GitHub Discussions** designed for?
    Select only one answer.
    - Tracking specific bugs and actionable engineering tasks with assignees.
    - Hosting open-ended community conversations, Q&A, announcements, and brainstorming outside of code Issues.
    - Storing compiled container images and npm packages.
    - Reviewing line-by-line diffs in a Pull Request.

60. Which GitHub security feature automatically creates Pull Requests to update outdated or vulnerable dependencies in your repository?
    Select only one answer.
    - GitHub Copilot
    - Dependabot
    - GitHub Pages
    - GitHub Gist

61. What is **Secret Scanning** on GitHub?
    Select only one answer.
    - A tool that encrypts all files in a public repository.
    - A feature that scans repositories for accidentally committed credentials, API keys, and tokens, alerting administrators and service providers.
    - A two-factor authentication app for mobile devices.
    - A feature that hides commit authors' email addresses.

62. What are **Branch Protection Rules** (or Rulesets) used for?
    Select only one answer.
    - To prevent anyone from cloning or viewing a public repository.
    - To enforce workflows on specific branches, such as requiring Pull Request reviews, passing status checks, or preventing force pushes.
    - To automatically delete branches every Monday.
    - To limit the number of files a branch can contain.

63. Which permission level on a repository allows a user to read and clone the repository, open issues, and submit pull requests, but NOT push directly to the repository?
    Select only one answer.
    - Admin
    - Write
    - Read
    - Maintain

64. How can you mention a specific user or team in a GitHub Issue or Pull Request comment so they receive a notification?
    Select only one answer.
    - Prefix their username or team slug with `#` (e.g., `#username`).
    - Prefix their username or team slug with `@` (e.g., `@username` or `@org/team`).
    - Enclose their username in double asterisks `**username**`.
    - Add their email address to the `.gitignore` file.

65. What is a **Release** on GitHub?
    Select only one answer.
    - A temporary branch created for fixing a typo.
    - A packaged version of software built on top of a Git tag, complete with release notes and optional compiled binary assets.
    - A notification sent when someone stars your repository.
    - A type of GitHub Organization billing plan.