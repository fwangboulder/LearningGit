# LearningGit
## Heading
```
# The largest heading
## The second largest heading
###### The smallest heading
```
# The largest heading
## The second largest heading
###### The smallest heading
##Styling text
```
**This is bold**
*italic*
~~mistaken~~
***bold and italic***
<sub> subscript</sub>
<sup>superscript</sup>
```
**This is bold**
*italic*
~~mistaken~~
***bold and italic***
<sub> subscript</sub>
<sup>superscript</sup>
## Quoting text and Quote code
```
>quote text, ```code block```.
```
>quote text
```
block
```
## Links
```
[link text](URL)
![This is image](URL)
```
[link text](URL)

![This is image](URL)




## Work with Github account
>Step 1 : Create SSH keys for all accounts

>Step 2 : Add SSH keys to SSH Agent

>Step 3 : Add SSH public key to the Github

>Step 4 : Create a Config File and Make Host Entries

>Step 5 : Cloning GitHub repositories using different accounts
```
cd ~/.ssh
ssh-keygen -t rsa -C "your-email-address" -f "github-username"
ssh-add -K ~/.ssh/github-username
pbcopy < ~/.ssh/github-username.pub
Githubaccount:Goto Settings > SSH and GPG keys > New SSH Key
touch config
open config

Here is content type in config:

#Your account
Host github.com-username
HostName github.com
User git
IdentityFile ~/.ssh/github-username

git clone git@github.com-{your-username}:{owner-user-name}/{the-repo-name}.git

git config user.email "email@gmail.com"
git config user.name "your name"
git remote add origin git@github.com-username:username
git push
git pull

```
## Reset git add

git reset

## add more in future!
