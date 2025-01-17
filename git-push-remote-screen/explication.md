# Documentation: Configuring Two Remotes and Git Alias

## Step 1: Adding a Second Remote

To add a second remote (`backup`), I ran the following commands:

```bash
git remote add backup https://github.com/Jun080/versionning-git-backup.git
git remote -v
```

Open add-remote.png to look at the screenshot

---

## Step 2: Configuring an Alias to Push to Two Remotes

To simplify pushing to both `origin` and `backup`, I configured a Git alias named `pushall` with the following commands:

```bash
git config alias.pushall '!git push origin && git push backup'
git pushall
```

This alias allows me to execute a single command (`git pushall`) to push changes to both remotes simultaneously.  

Open config-alias.png to look at the screenshot
