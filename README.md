# Configuring Git and GitHub on WSL2

## Create a GitHub Account

To work on and get credit for the labs and lessons that you work on during the
program, you will need to sign up for a GitHub account _if you don’t already
have one_.

### Action Item

1. Open the [GitHub signup webpage][] at https://github.com/join
2. Fill out the form and create your account
3. Verify the email address connected to your GitHub account

[GitHub signup webpage]: https://github.com/join

### Check Your Work

<iframe width="560" height="315" src="https://www.youtube.com/embed/mFZOVj8hago" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you were able to verify your email address, continue below.

## Configure Git and GitHub

Git is the tool that we’ll use to download and upload the work we do in labs and
lessons. To use Git without signing in every time, you can create a Secure Shell
(SSH) key and associate that to your GitHub account. Lastly, you will want to
run a few commands to make sure that when you use Git, you get the proper credit
for your work. This step will ask you to do work both in your browser and your
terminal.

### Action Item

1. Open the "Ubuntu" application using the "Start" menu
2. Type `git config --global color.ui true` and press `<Enter>`
3. Type `git config --global user.name` + `<Space>` + your name and press `<Enter>`
4. Type `git config --global user.email` + `<Space>` + the email address you
   used to sign up to GitHub and press `<Enter>`
5. Type `ssh-keygen` and press `<Enter>`, **for each prompt do not type anything**,
   just continue to press `<Enter>`
7. Type `cat ~/.ssh/id_rsa.pub | clip.exe` and press `<Enter>`. This will copy your SSH key to your clipboard
8. Open the [GitHub New SSH key form][ssh form] (https://github.com/settings/ssh/new)
   _(Note: you need to be logged in to GitHub to access that link.)_
9. Type "My personal PC" in the "Title" input field
10. Paste what’s on your clipboard from step seven in the "Key" input field
11. Click "Add SSH Key"

[ssh form]: https://github.com/settings/ssh/new

### Check Your Work

<iframe width="560" height="315" src="https://www.youtube.com/embed/ZosWXqhYD00" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you see your new SSH key beneath the "SSH keys" heading, continue to the next lesson, **Verify and Troubleshoot Your WSL2 Environment Setup**.
