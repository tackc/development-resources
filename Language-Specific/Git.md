# Git Resources

* [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)

* [Oh Shit, Git!?!](https://ohshitgit.com) - Fantastic git resource to fix git mistakes

* [Sync fork to original repo](https://digitaldrummerj.me/git-syncing-fork-with-original-repo/)

* Selectively choose portion of changes to stage: `git add --patch <filename>`

* [Git Docs](https://git-scm.com/docs)

* [Git Rebase](https://www.atlassian.com/git/tutorials/rewriting-history/git-rebase)

* [Git Forks and Upstreams](https://www.atlassian.com/git/tutorials/git-forks-and-upstreams)

* [Useful git commands](https://medium.com/better-programming/git-commands-to-live-by-349ab1fe3139)

* View contents of stash by running `git stash show -p` 
  * -p says that we want to see the actual content of the stash. Omitting it will show only the file names.

* Change Last Commit Message
  * `git commit --amend [-m '<message>']`
  * If the old commit had already been pushed, you’ll need to additionally run `git push --force-with-lease <remote> <branch>`
  * Note: As a general rule, and especially if you’re working with others, it’s important to be careful when making any changes to already pushed commits.

* Delete Last Commit but Keep the Changes - You’ve committed changes that you’d like to keep, but for whatever reason, you don’t want the commit itself.
  * `git reset HEAD^`
  * Note: The warning about making changes to already pushed commits holds here too!
  