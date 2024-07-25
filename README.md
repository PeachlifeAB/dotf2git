# dotf2git

**dotf2git** is a script for backing up your dot files to your own GitHub account.

## Setup

**Clone and Create Private Repository**:
1. Create a new private repository on your GitHub account (name it `dotf2git`)
2. Run the following command. Make sure to replace **YOUR_GITHUB_USER_NAME**.
    ```bash
    cd ~
    git clone git@github.com:PeachlifeAB/dotf2git.git
    cd dotf2git
    git remote set-url origin git@github.com:YOUR_GITHUB_USER_NAME/dotf2git.git
    git push -u origin main
    ~/dotf2git/backup
    ```
    
**IMPORTANT** Be sure to keep your new repository private so only you can access your config files.

## Usage

**Backup Dotfiles**: To sync and back up your dotfiles, run:
```bash
~/dotf2git/backup
```

## How it works
- The backup script will look for common files in your home directory and sync them to a branch named after your computer name (hostname) and push them.

## Missing some dot files?
Add the file name to whitelist.txt
