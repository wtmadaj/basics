1. [Running Locally](#RunningLocally)
    - [Node](#Node)
    - [Flutter](#Flutter)
2. [Git: SSH and HTTPS](#Git)
3. [MongoDB](#MongoDB)
4. [References](#References)


# Running Locally
## Node
>nodemon [jsfile]

to watch handlebar and js files (like .hbs):
>nodemon [jsfile] -e js,hbs

If package.json has a start script:
>npm run start [or other script name]

## Flutter
>flutter run

Run an alternate file:
>flutter run -t lib/otherFile.dart

Target a device with verbose logs:
>flutter run -v -d macos run

See available (running) devices:
>flutter devices 
<hr>

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
>git remote add origin https://github.com/wtmadaj/chat-app.git
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

<hr>

# Heroku
## Set up new app
>heroku create {name}

## Adding SSH Key to Heroku
>heroku keys:add ~/.ssh/[key].pub

## Push code to heroku to deploy
>git push heroku main

# MongoDB
Get to root
>cd ~

Print the working directory
>pwd

Start the local MongoDB instance
>/Users/Wes/mongodb/bin/mongod --dbpath=/Users/Wes/mongodb-data
>
>/usr/local/opt/mongodb-community/bin/mongod --dbpath=/Users/Wes/mongodb-data


# References
Chat App: https://github.com/andrewjmead/node-course-v3-code
