# dotf2git

**dotf2git** is a script for backing up your dot files to your own GitHub account.

## Setup

**Clone and Create Private Repository**:
1. Create a new **private** repository on your GitHub account, use default settings without README and .gitignore file.
2. Run the following command. Make sure to replace **YOUR_GITHUB_USER_NAME**.
    ```bash
    cd ~
    git clone git@github.com:PeachlifeAB/dotf2git.git
    cd dotf2git
    git remote set-url origin git@github.com:YOUR_GITHUB_USER_NAME/dotf2git.git
    git push -u origin main
    ~/dotf2git/backup
    ```

## Usage

**Backup Dotfiles**: To sync and back up your dotfiles, run:
```bash
~/dotf2git/backup
```

## Multiple computers
Supported. Just clone your private version of this repo and run `~/dotf2git/backup` on it.
The script will create a new branch for each computer.

## How it works
- The backup script will look for common dot files in your home directory and syncs the changes to a unique branch for each computer you use.

## Missing some dot files?
Add the file name to whitelist.txt
