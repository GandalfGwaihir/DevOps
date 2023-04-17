### SETUP

Configuring user information used across all local repositories

* To set a name that is identifiable for credit when review version history

    ```bash
     git config --global user.name “[firstname lastname]”
     ```
* To set an email address that will be associated with each history marker
    ```bash
    git config --global user.email “[valid-email]”
    ```
* To set automatic command line coloring for Git for easy reviewing
    ```bash
    git config --global color.ui auto
    ```
### SETUP AND INIT

Configuring user information, initializing and cloning repositories

* To initialize an existing directory as a Git repository
    ```bash
    git init
    ```
* To retrieve an entire repository from a hosted location via URL
    ```bash
    git clone [url]
    ```
### STAGE & SNAPSHOT

Working with snapshots and the Git staging area

* To show modified files in working directory, staged for your next commit
    ```bash
    git status
    ```
* To add a file as it looks now to your next commit (stage)
    ```bash
    git add [file]
    ```
* To unstage a file while retaining the changes in working directory
    ```bash
    git reset [file]
    ```
* To diff of what is changed but not staged
    ```bash
    git diff
    ```
* To commit your staged content as a new commit snapshot
    ```bash
    git commit -m “[descriptive message]”
    ```

### BRANCH & MERGE

Isolating work in branches, changing context, and integrating changes

* To list your branches, A * will appear next to the currently active branch
    ```bash
    git branch
    ```
* To create a new branch at the current commit
    ```bash
    git branch [branch-name]
    ```
* To switch to another branch and check it out into your working directory
    ```bash
    git checkout
    ```
* To merge the specified branch’s history into the current one
    ```bash
    git merge [branch]
    ```
* To show all commits in the current branch’s history
    ```bash
    git log
    ```
### SHARE & UPDATE
Retrieving updates from another repository and updating local repos

* add a git URL as an alias
    ```bash
    git remote add [alias] [url]
    ```
* fetch down all the branches from that Git remote
    ```bash
    git fetch [alias]
    ```
* merge a remote branch into your current branch to bring it up to date
    ```bash
    git merge [alias]/[branch]
    ```
* Transmit local branch commits to the remote repository branch
    ```bash
    git push [alias] [branch]
    ```
* fetch and merge any commits from the tracking remote branch
    ```bash
    git pull
    ```
### REWRITE HISTORY
Rewriting branches, updating commits and clearing history

* apply any commits of current branch ahead of specified one
    ```bash
    git rebase [branch]
    ```
* clear staging area, rewrite working tree from specified commit
    ```bash
    git reset --hard [commit]
    ```