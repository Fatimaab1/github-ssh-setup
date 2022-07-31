## SSH Documentation

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
