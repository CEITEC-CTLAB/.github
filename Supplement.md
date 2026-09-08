# Supplementary Material

1. [Markdown](#markdown)
2. [Glossary of Terms](#glossary-of-terms)
   1. [Git](#git)
   2. [Github](#github)
3. [Issue Time and Project Management](#issue-time-and-project-management)
4. [Calendar Versioning](#calendar-versioning)

## Markdown

When working on your code projects, you will come across [Markdown](https://www.markdownguide.org/getting-started/), a simple markup language used all over Github.
Use Markdown to format issues, pull requests, readmes, and other texts within your repositories.
Markdown is [easy to learn](https://www.markdownguide.org/basic-syntax/) while offering [plenty of tools](https://www.markdownguide.org/extended-syntax/) to communicate your ideas clearly and format your text into a neat document without much effort at all.
If in doubt, you can always refer to this [Markdown cheat sheet](https://www.markdownguide.org/cheat-sheet/).
Markdown processors are built into not only Github, but many popular IDEs, too, and even more programs offer Markdown plugins, so go wild!

## Glossary of Terms

### [Git](https://git-scm.com/docs/gitglossary)

- **[blame](https://git-scm.com/docs/git-blame)** - show the last revision and author of each line of a file.
- **branch** - a single line of development. Its latest commit is the *tip* of the branch, and it is referenced by the name *head*, or *HEAD* for the currently selected branch.
- **checkout** - update the *working tree*.
- **[clone](https://git-scm.com/docs/git-clone)** - create a copy of a repository
- **commit**
  - Noun: a single point in the history of the Git repository, uniquely identified by a *hash* calculated by Git using SHA-1 (Secure Hash Algorithm 1).
  - Verb: the action of storing a certain state of the repository in the Git history, thus updating *HEAD*.
- **fast-forward** - a special kind of merge. If merging branch *b* into branch *a* and if *b* is a descendant of *a*, *a* is simply updated to the state of *b* without the need to create another merge commit.
- **fetch** - get the *head* of a branch from a *remote* repository, without altering the local state of the repository.
- **merge**
  - Verb: bring the contents of another branch (from the same or different repository) to the current branch. Git attempts to automatically identifying and applying changes between the diverging branches, and in case of conflicts, it allows users to resolve them manually.
  - Noun: short for *merge commit*, a commit resulting from a successful merge, with the *tips* of the merged branches as *parents*
- **orphan** - getting on a currently non-existent branch. If a commit is made, it becomes a commit without a parent, starting a new history.
- **parent** - a logical predecessor of a *commit object*.
- **[prune](https://git-scm.com/docs/git-prune)** - remove all *unreachable* objects from the repository's object database. A typical use-case is removing references to upstream branches which do not exist anymore.
- **pull** - combination of a *fetch* and a *merge* operation
- **push** - the act of putting objects from a *local* branch into a *remote* branch (if the remote branch is an ancestor of the local branch) and updating the *remote* *head*.
- **reachable** - one object is reachable from another if there is a chain of references between the two (very simplified, see [here](https://git-scm.com/docs/gitglossary#def_reachable) for a detailed explanation)
- **rebase** - re-apply a series of changes from a branch to a different base than the current base state. Also resets the *head* of that branch to the result.
- **ref** - a name that points to an object or another ref.
- **remote** - also called *upstream*, this is a repository which tracks the same project as the local repository, but is not stored locally. Local and remote repositories can communicate through the *fetch* and *push* actions. The terms *remote* and *upstream* can also be used to refer to *branches*. The default remote repository is typically referred to as *origin*.
- **repository** - a collection of refs and a database of all objects reachable from these refs (more info [here](https://git-scm.com/docs/gitglossary#def_repository))
- **stage** - also called the *index*, this is in essence a collection of files that are being tracked by git, but not yet *commited* to the repository's history. The staging area is used to prepare changes before *committing* them.
- **[squash](https://git-scm.com/docs/merge-options)** - combine multiple commits into a single commit. Often used while *merging*.
- **tag** - a reference pointing to a specific object, typically a *commit*. It is not updated through commits, unlike *head*. Typically used to mark a certain point in the history of the repository, e.g., a release version.
- **working tree** - the collection of currently checked out files, i.e., *HEAD* and any uncommitted local changes, stored in the *working directory*

### [Github](https://docs.github.com/en/get-started/learning-about-github/github-glossary)

- **mention** - notify a person using their username with an @ in front.
- **access token** - a 'key' which you can generate for yourself to connect to github or its API through other applications.
- **assignee** - a user that is assigned to do a certain task (work on an *issue*, merge a *commit*)
- **base branch** - the branch you want to merge changes into, i.e., the target of a *pull request*
- **collaborator** - someone with read/write access to a repository, invited to contribute by the repository owner. The term *outside collaborator* refers to a person who was given access to an *organization's* repository, but is not a member of the organization.
- **fork** - a personal copy of a repository on another account than the original repository. Forks are useful for making custom changes to a public repository. You can also open *pull requests* from a fork to the original repository, which is handy in large, decentralized public projects.
- **gist** - a shareable file which can be edited, cloned, and forked on github, but is not a full-on repository. Can be *public* or *secret*, but secret gists can still be shared with anybody through a link.
- **issue** - a suggestion for a new feature or bug fix, a task, etc. It is a useful tool for basic tracking and work distribution within a code project. Each issue has its own discussion thread and additional tools to make working on the issue easier.
- **[keyword](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/using-keywords-in-issues-and-pull-requests)** - specific words which link *pull requests* with *issues* when used in the description of a *pull request*.
- **label** - tags used to categorize *issues* and *pull requests*.
- **license** - a document specifying how the code within your repository can be used, and what the restrictions for this are. Especially relevant for public repositories.
- **milestone** - tools to track progress on *issues* and *pull requests*.
- **organization** - a group of users which contains *repositories*, *projects*, and *teams*.
- **[project](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects)** - a suite of project management tools within Github. It includes roadmaps, [kanban boards](https://www.atlassian.com/agile/kanban), and seamless integration of *issues* and *pull requests*.
- **public repository** - a repository which can be accessed by anyone (even people without a Github account). In contrast, a private repository is only accessible for collaborators invited by the repository owner.
- **pull request** - a proposal for changes to a repository, which is submitted by a contributor. The request is reviewed and then accepted or rejected (outright or with a request for further changes) by other collaborators. Pull requests have their own discussion threads, and can be linked to *issues* using *keywords*. If approved, pull requests are typically closed by *merging* the proposed changes into the *base branch*.
- **release** - a Github-specific way of packaging software for end-users. A release contains an archive of the source code along with any compiled binaries and other associated files added by the creator of the release. Releases are associated with specific *commits* through *tags*.
- **review** - comments on pull requests from collaborators, which can range from discussion to corrections, suggestions, or requests for changes in specific lines of code, parts of files, etc.
- **team** - a group of members within an organization with defined access permissions to the organization's repositories.
- **topics** - located in the *About* section of a repository, topics are labels used to categorize repositories.
- **watch** - a user can choose to watch repositories or issues to get notified when changes are made.

## Issue Time and Project Management

- Not always necessary, but useful for complex issues or larger teams.
  - Consult with seniors about the use of this feature.
- Add Milestones to Hit While Solving the Issue.
  - `Issues` → `Milestones` → `New milestone`.
  - Set a title, description, and due date for the milestone.
  - Link the milestone to the relevant issue.
- Add Issues to project roadmap to visualize progress and deadlines
  - [`Projects`](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects) are project/time management tools integrated in GitHub.

## Calendar Versioning

If you are going to create releases for your codebase/project, it is good practice to identify each release using a unique and easily decipherable version tag.
The specific versioning convention will depend on the project you are working with and the consensus of your team.

We recommend tagging release versions using a version of [**Calendar Versioning**](https://calver.org/) (CalVer).
In CalVer, releases are marked by date of publication in the format `vYY.MM.DD` (year.month.day of the release, e.g., v24.09.04).
The preceding `v` is not strictly necessary, but it helps clearly communicate that this is a version number. The year-month-day format sorts your releases chronologically without the need to keep track of an arbitrary version counter (as is the case in [semantic versioning](https://semver.org/)).

In some cases, you may want to indicate that the current release is not a stable one, but rather a preliminary or testing version.
You can indicate this in the version tag by adding a suffix such as `-alpha`, `-beta`, or `-pre` (e.g., `v24.09.05-beta`).
On very rare occasions, it might be necessary to release multiple versions on the same day.
You can distinguish these versions by adding a letter suffix to the version tag, e.g., `v24.09.05a` and `v24.09.05b`.

<!-- TODO code coverage monitoring -->

<!-- TODO what if bug - just fix it -->

<!-- Automated testing -->

<!-- TODO put appendix in separate file - supplement -->