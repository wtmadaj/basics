# Git
## View SSH folder
>ls -al ~/.ssh

## Start SSH Agent
>eval "$(ssh-agent -s)"

## Add Key to Agent
>ssh-add -K ~/.ssh/id_rsa

# Using HTTPS for Git
To prevent starting ssh agent each time, use GCM by changing the connection to HTTPS
>git remote set-url origin https://github.com/[username]/[repo-name].git

This lets GCM manage credentials and connections for git operations.

## Git commands
Initialize repo:
>git init
>
>git add .
>
>git status
>
>git commit -m "put message text here"

Then create repo in github
Then:
>git remote add origin https://github.com/[username]/github-repo-name.git
>
>git branch -M main
>
>git push -u origin main


Show git details for repo
>git config --list

## References
- https://github.com/GitCredentialManager/git-credential-manager
- https://linuxize.com/post/how-to-change-git-remote-url/
- https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories