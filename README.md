# SSH setup between our Localhost and Github
- Open Git Bash as Administrator
- cd to the .ssh folder
- Enter the following command: `ssh-keygen -t rsa -b 4096 -C "amurphy@spartaglobal.com"`
- For each of the subsequent questions asked, press `Enter`
- In GitHub, go to Settings and click `SSH and GPG Keys`, then click `New SSH Key`
- Name the key, e.g. `SRE_CICD`
- In Git Bash, do the following command: `cat id_rsa.pub`, and copy the results - DO NOT COPY WHITESPACE
- Paste the result into the `Key` input box
- Click `Add SSH key`
- Add a new repo
- Above the commands for connecting the repo to your localhost, GitHub will be automatically using `HTTP` - click `SSH`
- In Git Bash, make a new directory where you want your repo to be
- Follow the commands provided by GitHub to connect your current directory to the repo
> If there is a problem verifying your git commit or git push, you might have to use the following commands to attach your name and GitHub email address to your commits:
> git config --global user.email "you@example.com"
> git config --global user.name "Your Name"
> Then repeat the command that had a problem
