# Git

## Definitions

*branch* - Branches are not used in the Git session in this curriculum, but are a frequently used feature of Git. A branch is an alternative timeline of commits, usually used to add a new feature or some other substantive change to a repository. Once the feature or change is complete, the branch can be reintegrated with the main timeline, which is usually called "master."  

*clone* - A local copy of a repo. cloning lets you work offline.

*cloning* - Cloning creates a local copy of a remote repository, then connects the local with the remote. After you clone a repository on GitHub, for example, you'll have a new folder on your computer that is a copy of the files in the remote repository. In addition, you'll have access to the history of the project (accessible through commands such as `git log`) and the local repository will be connected to the remote repository (called "origin"). This means you can push changes to the remote repository or pull changes to your local repository.  

*directory* - In your GUI, a folder. A file system data structure.

*fork* - The way others interact with and can modify your Github repos. Forking makes a copy of someone's repo in a way that connects back to the original repo, but lets you modify it without altering the original.

*forking* - Forking allows you to freely make changes to a copy of a repository without affecting the original repository. You can however, propose changes (through a *pull request*) to incorporate into that original repository.  

*git* - Git is a version control tool. It lives on your local computer and can be accessed through the command line.  

*GitHub* - GitHub is a proprietary cloud service, like Twitter or Google Docs, that hosts git repositories online. GitHub also provides issue tracking and other collaboration features.  

*GUI* - graphical user interface, or anything on a computer or browser where you can point at an icon and click. In contrast to the command line, where you give direct commands to the computer by typing them out.

*local* - An adjective describing the machine you're sitting in front of. "Your local machine" usually translates to "your laptop." In Git, a local repository is a repository on your machine.  

*markdown* - Markdown is a specific markup language designed to be readable as code, not just when it's displayed. That makes it fun to write in, at least compared to HTML. Markdown is provides a readable syntax for a subset of HTML, such as headings, lists, and links. These tutorials are written in markdown.  

*markup* - Markup languages allow you to format things, whether they're documents, posters, or websites. HTML is a markup language, as is LaTeX.  

*master* - The default branch, and typically the primary branch of a project. When a new repository is created with `git init`, it has one branch, and that branch is called "master."

*merge conflict* - If, when attempting to merge, there is a line that has been changed by both parties, you will experience a merge conflict. This means that Git needs your manual intervention to decide which of the two changes will be the canonical or accepted change. A merge conflict is resolved by editing the conflicting files with a text editor, then adding and committing to resolve the merge.  

*merging* - If you've advanced the timeline of a repository by making commits, and someone else has advanced the timeline of a remote version of the repository, when you attempt to pull in the remote changes you will be prompted to merge the two timelines. In most cases this is an automatic process that reconciles the two timelines.  

*origin* - In Git, the default remote repository. When you clone a remote repository—that is, make a local reposotry based on it—the remote repository is automatically added as "origin."

*pull request* - A pull request is a set of proposed changes to a repository. If you wish to contribute to an open-source project, the most common method is by proposing changes through pull requests.  

*pull* - Accepting and taking changes that were made to a remote repository, possibly by someone else, and updating your local repository to match.  

*push* - Pushing means sharing local changes with a remote repository. When you push local commits, the history of the remote repository is updated to match your local timeline.

*remote* - An adjective describing a computer that is somewhere else. A "remote machine" is a machine you do not have physical access to, but might have access through a means such as the internet. In Git, a remote is a repository that is not on your computer, but is connected to your local repository. You can add new remotes with the `git remote add` command, and change them with the `gitremote set-url` command.

*repo* - Short for repository.  

*repository* - A folder that is currently being tracked by Git. The folder could be on your local machine or it could be on a service such as GitHub. The tracking information that makes a normal folder into a Git repository is contained in a hidden folder, called `.git`, that lives in the repository.

*version control system (VCS)* - A tool for keeping track of versions of files in a project. They allow for collaboration in a team, storing work in multiple locations, and reverting back to a previous state of the project.

*working directory* - A group of files you're in the process of editing.

___
Sources and further reading:
- [http://git-scm.com/book/en/v2/](http://git-scm.com/book/en/v2/)
- [http://help.github.com/articles/](http://help.github.com/articles/)
- [http://help.github.com/articles/github-glossary/](http://help.github.com/articles/github-glossary/)
