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
