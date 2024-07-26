# dotf2git

A simple tool for backing up your dot files to your own GitHub account.

## Initial setup

1. Create a new **private** repository on your GitHub account. Don't add any files to it.
2. Open a Terminal and run:

```bash
cd ~ && git clone git@github.com:PeachlifeAB/dotf2git.git && dotf2git/backup
```

This will set the remotes up for you and ensure you can easily get latest features and bug fixes.

## Use

To sync and back up your dotfiles, run:

```bash
~/dotf2git/backup
```

## Get latest features

```bash
~/dotf2git/update
```

This will pull latest upstream changes to your personal version of this repo.

## Multiple computers

**Supported**
Just clone your private version of this repo on each computer and run:

```bash
~/dotf2git/backup
```

The script will create a new branch named after each computer’s hostname, ensuring separate backups for each machine.

## Missing some dot files?

Just add the file name to `whitelist.txt`
If you think it should be included for everyone, please add an [issue](https://github.com/PeachlifeAB/dotf2git/issues/new/choose)
