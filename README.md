# HTTPS & SSH Documentation

## Repository setup with HTTPS

**Step 1:** Once you are logged in to your Github account navigate to your profile and create a new repository 

**Step 2:** Enter a repository name of your choice, then set it to public and click create repository at the bottom of the page

**Step 3:** At the top of the page you will see a blue box tittle Quick setup, then select HTTPS

**Step 4:** On the same page you will see the following commands you will need to follow 

`git init`

`git add .`

`git commit -m "first commit"`

`git branch -M main`

`git remote add origin "your https link here"`

`git push -u origin main`

**Step 5:** once you have run the commands on the terminal, refresh your GitHub page and you will be directed to your new repository. 


## Repository setup with SSH

**Step 1:** Create a new Github repository.

**Step 2:** Click on the green code button on the top right and copy the SSH link provided.

**Step 3:** Open the terminal and enter the following command:
This will bring you to your home location 
$ cd 

**Step 4:** Create a folder if it doesnt already exist
$ mkdir .ssh

**Step 5:** Generate a new ssh key and replace text inside " " with your email

`$ ssh-keygen -t ed25519 -C "your_email@example.com"`

**Step 6:** You will then be asked to enter a passphrase
````
Note: Leave empty for no passphrase (click enter x2)
````
**Step 7:** Add your new key to the shh-agent

`$ eval "$(ssh-agent -s)"`

**Step 8:** Enter file name to save your key to the shh-agent
````
Note: Replace ID with your file name
````
`$ ssh-add -K ~/.ssh/id_ed25519`


Step 9: Randomart image will be generated for the key 

Step 10: To check if files exists use the following command

`$ ls`
