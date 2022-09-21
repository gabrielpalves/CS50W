## GitHub
Website that stores git repositories (folders with code inside).

You can fork a repository make an exact copy of another's repository.

## git
git is a command line tool that allow us to:
- keep track of changes in the code
- synchronize code between different people
- test changes to code without losing the original
- revert back to old versions of code

### Commands

#### init
> Initializes an empty git repository in your current folder.

#### clone
> Clone your repository to your local machine
> 
> `git clone <repoURL>`

#### pull
> Bring down the changes that some of your colleagues might have made and pushed up to the repository
> 
> pull from branch main to sync: `git pull origin main --allow-unrelated-histories`
> 
> `--allow-unrelated-histories` allows git to merge two different projects with different histories

#### fetch
> Fetch remote branches: `git fetch --all`

#### add
> Add file(s) to track the next time a commit is done.
> 
> `git add <filename>` or `git add .` to add all modified/created files

#### commit
> Save a snapshot of the current state of the repository, keeping track of any of the changes added using `git add`
> 
> `git commit -am "message"`
> 
> `-a` combines the `git add` part
> 
> `-m "message"` to add some short note to know the changes made
> 
> To reset changes in brach before commit: `git reset --hard`

#### status
> Tells what's currently happening in the current repository.
> 
> `git status`

#### log
> Check log history (`git log`). Describes each of the commits.

#### push
> Push the changes to the remote repository: `git push` if the branch is already in the remote repository. Else, use:
> 
> `git push -u origin <branch>`
> 
> or
> 
> `git push --set-upstream origin <branch>`
> 

#### branch
> Create a branch in your local machine: `git branch <new-branch>` or `git checkout -b <branch>`
> 
> Delete a branch with: `git branch -d <branch>`
> 
> List the branches with: `git branch`
> 
> List the remote branches with: `git branch -r`

#### checkout
> Let git know that any change made will be in that specific branch
> 
> `git checkout <branch>`

#### undoing commits
> `git revert` creates a commit with the exact opposite changes of whichever commit you would like to undo. Commit ID remains unchanged. Safest way.
> 
> `git reset --hard <ID of commit>`
> 
> `git reset --hard origin/main`
> 
> `git commit --amend` lets you modify your last commit. Can be used to change commit message
> 
> `git cherry-pick` changes the commit ID

### Branching
It is important to not keep a linear track of your changes, because things can get complicated in bigger projects and to alter something that was already done can be difficult. That's where branching comes in.

The focus of your repository, the current state of it, is designated by `HEAD`.

## GitHub pages
Create a new repository: `<yourusername>.github.io`. Push an `index.html` in it and then access your website. Done.