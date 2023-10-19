# Git
## View SSH folder
```bash
ls -al ~/.ssh
```

## Start SSH Agent
```bash
eval "$(ssh-agent -s)"
```

## Add Key to Agent
```bash
ssh-add -K ~/.ssh/id_rsa
```

# Using HTTPS for Git
To prevent starting ssh agent each time, use GCM by changing the connection to HTTPS
```bash
git remote set-url origin https://github.com/[username]/[github-repo-name].git
```

After authenticating via browser or token, this lets GCM manage credentials and connections for git operations.

## Git commands
Initialize repo:
```bash
git init
git add .
git status
git commit -m "commit message here"
```

Then create repo in github
Then:
```bash
git remote add origin https://github.com/[username]/[github-repo-name].git
git branch -M main
git push -u origin main
```

Show git details for repo
```bash
git config --list
```

## References
- https://github.com/GitCredentialManager/git-credential-manager
- https://linuxize.com/post/how-to-change-git-remote-url/
- https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories