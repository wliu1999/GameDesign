# Janaurius ReadMe

Hey guys! Here's some quick instructions to help y'all get set up for local development.

Instructions for Windows setup:

1. Open command prompt and use the `cd` command to navigate to a folder that you want to store your SSH key in.
2. Use the command `ssh-keygen -t rsa -f ~/.ssh/id_rsa` to create an SSH key. This will allow you to connect to the shared github repo. Ignore this if you already have an ssh key.
3. With your file explorer, go to the folder you chose earlier. The command will have generated a folder called `.ssh`. Open it up.
4. There should be a file within that folder called `id_rsa.pub`. Right click it, and use a text editor like notepad to open it, and copy it to your clipboard. Attempting to open this with Microsoft Publisher WILL NOT WORK.
5. Go to the *[Github settings page](hhttps://github.com/settings/keys)* and click the `New SSH key` button. Set a title that you'll remember, and paste the SSH key in the appropriate field.
6. Open up Godot and create a new project.
7. Open command prompt again and use the `cd` command to navigate to your Godot project.
8. Use `git init` to create a new local git repository within that project file.
9. Use `git remote add origin git@github.com:wliu1999/Janaurius.git` to connect this local git repo to the shared one. 
10. Use `git pull origin main` to download the starter code from the shared git repo.