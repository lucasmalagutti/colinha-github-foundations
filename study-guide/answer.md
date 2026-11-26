# GitHub Foundations - Answer Key

 1. **Correct Answer:** Git is a distributed version control system, while GitHub is a cloud-hosted platform built around Git.
    * *Explanation:* Git is the underlying version control software run locally, while GitHub is a cloud-based hosting service that adds collaboration tools around Git repositories.

 2. **Correct Answer:** Distributed Version Control System (DVCS)
    * *Explanation:* In a DVCS like Git, every contributor clones the full repository, including its complete history, rather than relying solely on a central server.

 3. **Correct Answer:** Version Control as a Service (VCaaS)
    * *Explanation:* GitHub delivers version control and repository hosting over the cloud as a managed service (VCaaS).

 4. **Correct Answer:** git init
    * *Explanation:* Running `git init` creates a hidden `.git` subdirectory in your current directory, initializing a new repository.

 5. **Correct Answer:** To download a full copy of an existing remote repository to your local machine.
    * *Explanation:* `git clone` downloads the source code, branches, and full commit history from a remote URL to your local machine.

 6. **Correct Answer:** git add
    * *Explanation:* `git add` promotes changes from the working directory into the staging area (index) in preparation for a commit.

 7. **Correct Answer:** git status
    * *Explanation:* `git status` displays which branch you are on, which changes are staged, which are unstaged, and which files are untracked.

 8. **Correct Answer:** git commit
    * *Explanation:* `git commit` captures a snapshot of the currently staged changes and stores it permanently in the local Git history.

 9. **Correct Answer:** Sends committed changes from a local branch to a remote repository.
    * *Explanation:* `git push` uploads local commits to the corresponding branch on a remote repository such as GitHub.

10. **Correct Answer:** git pull
    * *Explanation:* `git pull` is a combination of `git fetch` followed by `git merge`, downloading remote commits and integrating them into your active branch.

11. **Correct Answer:** git log
    * *Explanation:* `git log` lists the commits made in the repository in reverse chronological order along with commit hashes, authors, dates, and messages.

12. **Correct Answer:** To list, create, or delete branches in a repository.
    * *Explanation:* `git branch` manages local branches without switching your working directory (unlike `git checkout` or `git switch`).

13. **Correct Answer:** git remote
    * *Explanation:* `git remote` allows you to view, add, rename, or remove connections to remote repositories (commonly named `origin`).

14. **Correct Answer:** It combines the commit history of one branch into another active branch.
    * *Explanation:* `git merge` integrates changes from a specified branch into your currently checked-out branch.

15. **Correct Answer:** When you need to temporarily shelve uncommitted changes so you can switch branches cleanly.
    * *Explanation:* `git stash` saves dirty working directory changes onto a stack and reverts the working directory to match the `HEAD` commit.

16. **Correct Answer:** git reset
    * *Explanation:* Running `git reset` (or `git reset HEAD <file>`) unstages files while preserving your modifications in the working directory.

17. **Correct Answer:** To authenticate securely with GitHub over Git without entering a username and password on every operation.
    * *Explanation:* SSH keys use asymmetric cryptography to authenticate your machine securely with GitHub over SSH.

18. **Correct Answer:** Creating a dedicated feature branch from `main`, committing changes, opening a Pull Request, and merging after review.
    * *Explanation:* GitHub Flow is a lightweight, branch-based workflow centered around creating branches from `main` and collaborating via Pull Requests.

19. **Correct Answer:** Because `main` serves as the single source of truth from which new branches are created and production releases are made.
    * *Explanation:* Keeping `main` stable and deployable ensures that any new branch starts from working code and releases can happen at any time.

20. **Correct Answer:** REST API and GraphQL API
    * *Explanation:* GitHub provides both a traditional REST API and a flexible GraphQL API (v4) for automating workflows and querying platform data.

21. **Correct Answer:** It allows clients to request the exact data structure they need in a single request, avoiding over-fetching or under-fetching.
    * *Explanation:* GraphQL lets you specify exact fields across nested resources in one query, reducing bandwidth and round-trip API calls.

22. **Correct Answer:** The official suite of client libraries and SDKs provided by GitHub to interact with its APIs in multiple programming languages.
    * *Explanation:* Octokit provides official SDKs (for JavaScript/TypeScript, Ruby, .NET, etc.) to simplify authentication and requests to GitHub's REST and GraphQL APIs.

23. **Correct Answer:** GitHub Desktop
    * *Explanation:* GitHub Desktop is an official GUI client that simplifies cloning, branching, committing, and creating Pull Requests visually.

24. **Correct Answer:** Triage notifications, review and merge Pull Requests, and manage Issues on the go.
    * *Explanation:* GitHub Mobile is designed for lightweight collaboration, code review, issue triage, and notification management from iOS and Android devices.

25. **Correct Answer:** Personal account
    * *Explanation:* Every person using GitHub signs in to a Personal account, which owns personal repositories and can belong to Organizations.

26. **Correct Answer:** To provide shared ownership of repositories where businesses or open-source communities can collaborate with granular team permissions.
    * *Explanation:* Organizations allow multiple users to collaborate across shared repositories with role-based access control and nested teams.

27. **Correct Answer:** Enterprise account
    * *Explanation:* An Enterprise account acts as an umbrella over multiple Organizations, providing unified billing, SAML SSO, and policy enforcement.

28. **Correct Answer:** GitHub Free
    * *Explanation:* GitHub Free offers unlimited public and private repositories with unlimited collaborators for individual users.

29. **Correct Answer:** Advanced insights, GitHub Pages on private repositories, and increased GitHub Actions minutes and Packages storage.
    * *Explanation:* GitHub Pro upgrades a personal account with expanded CI/CD minutes, storage quotas, code owners, and private GitHub Pages sites.

30. **Correct Answer:** GitHub Team
    * *Explanation:* GitHub Team is designed for organizations needing team access controls, required reviewers, protected branches, and increased Actions/Packages quotas.

31. **Correct Answer:** Enterprise-grade security, SAML single sign-on (SSO), advanced auditing, and options for Enterprise Cloud or Enterprise Server.
    * *Explanation:* GitHub Enterprise provides compliance, centralized identity management (SAML/EMU), audit log streaming, and self-hosted deployment options.

32. **Correct Answer:** GitHub's extension of standard Markdown that adds features like task lists, tables, strikethrough, and automatic URL linking.
    * *Explanation:* GFM builds on CommonMark to add developer-focused formatting features used across Issues, Pull Requests, Comments, and READMEs.

33. **Correct Answer:** Using `[x]` and `[ ]` preceded by a list marker such as `- [ ] Task`.
    * *Explanation:* Adding `- [ ]` creates an interactive checkbox that users can click directly in the GitHub UI to toggle completion.

34. **Correct Answer:** Mermaid code blocks (` ```mermaid `)
    * *Explanation:* GitHub natively renders Mermaid diagrams inside fenced code blocks tagged with `mermaid`.

35. **Correct Answer:** GeoJSON (`.geojson` / `.topojson`)
    * *Explanation:* GitHub automatically converts `.geojson` and `.topojson` files (or `geojson` code blocks) into interactive maps.

36. **Correct Answer:** `.stl` (ASCII or binary STL)
    * *Explanation:* GitHub includes a built-in WebGL viewer that renders `.stl` 3D models interactively in the browser.

37. **Correct Answer:** GitHub uploads the asset to its CDN and automatically inserts the corresponding Markdown link into the comment.
    * *Explanation:* Dragging and dropping supported images, videos, or documents uploads them to GitHub's asset hosting without polluting your Git repository history.

38. **Correct Answer:** On the main front page of the repository below the list of files and directories.
    * *Explanation:* GitHub automatically detects a root `README.md` (or one in `.github/` or `docs/`) and displays it on the repository landing page.

39. **Correct Answer:** Clearly explain what the project does, why it is useful, how to install/use it, and how others can contribute.
    * *Explanation:* A well-structured `README.md` serves as the front door of a project, helping visitors quickly understand and adopt it.

40. **Correct Answer:** Insights > Pulse
    * *Explanation:* The Pulse view summarizes recent activity—including merged/open Pull Requests and closed/open Issues—over a chosen timeframe.

41. **Correct Answer:** Insights > Contributors
    * *Explanation:* The Contributors graph ranks repository contributors by commit volume and displays additions/deletions over time.

42. **Correct Answer:** To identify the manifest and lockfiles in a repository and list all direct and transitive packages the project depends on.
    * *Explanation:* The Dependency Graph parses supported package manifests to map dependencies and power Dependabot alerts.

43. **Correct Answer:** Insights > Community Standards
    * *Explanation:* Community Standards displays a checklist of recommended open-source documentation files such as `README`, `LICENSE`, `CONTRIBUTING`, and `CODE_OF_CONDUCT`.

44. **Correct Answer:** A personal copy of another user's or organization's repository under your own GitHub account.
    * *Explanation:* Forking creates an independent copy on GitHub so you can experiment or prepare contributions without needing write access to the original repository.

45. **Correct Answer:** By opening a cross-repository Pull Request from your fork's branch to the upstream repository's branch.
    * *Explanation:* Cross-repository Pull Requests allow maintainers of the upstream repository to review and merge contributions coming from external forks.

46. **Correct Answer:** To specify intentionally untracked files and directories (such as build artifacts or `.env` files) that Git should ignore.
    * *Explanation:* `.gitignore` prevents temporary files, dependencies (`node_modules/`), and sensitive local configuration files from being accidentally staged or committed.

47. **Correct Answer:** A simple, lightweight way to share code snippets, notes, or single files, backed by its own Git repository.
    * *Explanation:* Gists can be public or secret, support revision history, and can be cloned or embedded on external websites.

48. **Correct Answer:** GitHub Pages
    * *Explanation:* GitHub Pages builds and hosts static HTML/CSS/JS websites directly from a repository branch or via a GitHub Actions workflow.

49. **Correct Answer:** Watching subscribes you to notifications about repository activity, while Starring bookmarks the repository and shows appreciation.
    * *Explanation:* Starring adds a repo to your saved Stars list, whereas Watching controls your notification preferences (e.g., Participating, All Activity, or Ignore).

50. **Correct Answer:** `LICENSE` (or `LICENSE.md`)
    * *Explanation:* Including a `LICENSE` file clarifies copyright and grants explicit permissions for others to use, modify, or distribute the project.

51. **Correct Answer:** It automatically requests reviews from designated individuals or teams when Pull Requests modify specific files or directories.
    * *Explanation:* Defined using path patterns (similar to `.gitignore`), `CODEOWNERS` ensures the right subject-matter experts review changes to sensitive areas of the codebase.

52. **Correct Answer:** To categorize, filter, and prioritize issues and pull requests (e.g., `bug`, `enhancement`, `documentation`).
    * *Explanation:* Labels provide color-coded metadata tags that make triaging and searching Issues and PRs much faster.

53. **Correct Answer:** A way to group related Issues and Pull Requests together to track progress toward a specific goal, release, or sprint.
    * *Explanation:* Milestones include an optional due date and automatically calculate a completion percentage based on closed vs. open items.

54. **Correct Answer:** `Fixes #42` (or `Closes #42`)
    * *Explanation:* Keywords like `Fixes`, `Closes`, or `Resolves` followed by an issue number automatically close the linked issue when the PR is merged into the default branch.

55. **Correct Answer:** A Pull Request that signals work is still in progress and cannot be merged until it is marked as "Ready for review."
    * *Explanation:* Draft PRs allow early feedback and CI checks without triggering code-owner review notifications or allowing accidental merges.

56. **Correct Answer:** Squash and merge combines all commits from the Pull Request branch into a single commit on the base branch.
    * *Explanation:* Squashing keeps the `main` branch history clean and linear by condensing work-in-progress commits into one atomic commit.

57. **Correct Answer:** GitHub Codespaces
    * *Explanation:* Codespaces spins up containerized cloud development environments configured via `devcontainer.json`, accessible in a browser or VS Code.

58. **Correct Answer:** Automating software development workflows, including CI/CD pipelines, triggered by GitHub events.
    * *Explanation:* GitHub Actions uses YAML workflow files in `.github/workflows/` to run builds, tests, deployments, and repository automation.

59. **Correct Answer:** Hosting open-ended community conversations, Q&A, announcements, and brainstorming outside of code Issues.
    * *Explanation:* Discussions keeps non-actionable questions and community threads separate from actionable bug reports and feature tasks in Issues.

60. **Correct Answer:** Dependabot
    * *Explanation:* Dependabot monitors your Dependency Graph for security advisories and version updates, automatically opening Pull Requests with updated dependency versions.

61. **Correct Answer:** A feature that scans repositories for accidentally committed credentials, API keys, and tokens, alerting administrators and service providers.
    * *Explanation:* Secret Scanning detects known token patterns in commits and issues—and with Push Protection enabled, can block secrets from being pushed in the first place.

62. **Correct Answer:** To enforce workflows on specific branches, such as requiring Pull Request reviews, passing status checks, or preventing force pushes.
    * *Explanation:* Branch Protection Rules and Rulesets safeguard critical branches like `main` from unreviewed changes, failing tests, or accidental deletion.

63. **Correct Answer:** Read
    * *Explanation:* The `Read` role is ideal for non-code contributors or external users who need to view code, open issues, and participate in discussions without modifying repository contents directly.

64. **Correct Answer:** Prefix their username or team slug with `@` (e.g., `@username` or `@org/team`).
    * *Explanation:* Using `@mentions` sends a notification to the referenced user or team members, drawing their attention to the conversation.

65. **Correct Answer:** A packaged version of software built on top of a Git tag, complete with release notes and optional compiled binary assets.
    * *Explanation:* Releases provide a user-friendly way to distribute versioned software snapshots, changelogs, and downloadable binaries on GitHub.