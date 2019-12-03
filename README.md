# GitHub Tutorial

_by Giselle Tapia_

---
## Git vs. GitHub
The differenece of Git vs. Github
Git| Github
---|---
Version control : keeps "snapshots" of your code|To send to git do <git add .> then <git commit -m "comment">
Used to learn and understand | The website where everything gets stores (like "iCloud")
Git does not require github|Easily collaborate on files 
Git is like a photographer (meaning you can make changes, add and delete things)|GitHub is a place that stores your “pictures” (where your code is saved and where your commits live)
Basic work flow Git + directories or files (when we finally initialize git its called a repository)| Basic work flow for Github + Either you start from a new repository or you use one someone already created

### Github:


---
## Initial Setup
When making a github account 
1. Go to github.com 
2. Create an account
- For your username if you are a HSTAT student use the first part of your email and last four digets of your osis number (firstnameLastinitialLast4digetsofosisnumber Example:johnS5893)
- the password could be your osis number or something simple enough for you to rememmber
3. Next step is to set up your ide on https://ide.cs50.io/
- for the rest of the steps follow the instructions in the link below
    -https://docs.google.com/presentation/d/1bXBAxCa_U7NXVYxXZh3P34lhIrBNzdDVksiqqgOw4uE/edit#slide=id.g25b1b888c_00

SSH KEY: 
# What it is?
It is a command that provides secure encrypted connection between an insecure network and its used for terminal access and to provide automatic public-private key pairs


---
## Repository Setup
    git init
Initialize git in our directory (now called a repository) for version control
    -Only do it once at the beginning 
    
    git add .
adds current directories (all files that  have changed including the deleated ones and renamed)

    git commit -m ""
short specific message that should be in present-tense and describes what was motified in the snapshot.

---
## Workflow & Commands
    status
optional yet recommended command to see which files are staged for the community (they will show up green)

    add
adding files that have been changed or modified 
    - RED (not staged)
    - GREEN (staged)
    
    commit
To commit is to modify you code and the command you use is git commit -m ""

    push
Git push is when you send your code or snapshot into a new server


---
## Rolling Back Changes
    undo
To undo a command you do 

    edit
You can always edit on your ide or on the github website

    add/commit/push
You have to do git addd . to add what you changed to the current directory and then you do git commit -m "" to commit these changes and write a message to remin d you what changes you made to your code. After you push the command to your local repo using git push -u origin master