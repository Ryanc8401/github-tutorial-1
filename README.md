# GitHub Tutorial

_by Ryan Chen_

---
## Git vs. GitHub
The difference between Git vs. Github
Git| Github
---|---
Version control | keeps "snapshots" of your code|To send to git do <git add .> then <git commit -m "comment">
Used to learn and understand | The website where everything gets stores (like "iCloud")
Git does not require github|Easily collaborate on files 
Git is like a photographer (meaning you can make changes, add and delete things)|GitHub is a place that stores your “pictures” (where your code is saved and where your commits live)
Basic workflow Git + directories or files (when we finally initialize git its called a repository)| Basic workflow for Github + Either you start from a new repository or you use one someone already created

_What is the Git and Github?_

Git and GitHub are separate from one another even though they are used together. They may have the word "Git" but they function completely different from one another. Git acts more like a tool that keeps track of the changes you make while you're programming where you're able to look back what you've done. On the other hand, Github is used is a server that stores all your information digitally so you can access it anywhere rather than locally where it only available in your laptop/device.

Git | GitHub
---|---
Access Locally | Access Globally
Doesn't requires wifi | Requires wifi
It's on your computer | Collaboration with other

_What is a repo? Local vs Global?_

Repo is a short acronym for a repository, but you would wonder what is a repo and what does it do. A repository is a place where information can be stored and can be accessed later on. In this case, a repo is stored in GitHub where your project can be accessed anywhere with connection with wifi. This leads up to the questions what the difference between a local repo and a global repo. A local repo can only be accessible within the device that you store the information in and in order to share it you either have to store it within a server, but with a global repo, you can store it and access it in a different computer that isn't you own which is convenient.


---
## Initial Setup
When making a github account 
1. Go to github.com 
2. Create an account
- For your username, if you are an HSTAT student use the first part of your email and last four digits of your osis number (firstnameLastinitialLast4digetsofosisnumber Example:johnS5893)
- the password could be your osis number or something simple enough for you to remember
3. Next step is to set up your ide on https://ide.cs50.io/
- for the rest of the steps follow the instructions in the link below
    -https://docs.google.com/presentation/d/1bXBAxCa_U7NXVYxXZh3P34lhIrBNzdDVksiqqgOw4uE/edit#slide=id.g25b1b888c_00

### Step 0: Get a github account

Before we start using git and everything else we need to get you setup and prepare so we can dive deep into this tutorial. This is an additional step you need to do before you get start. If you don't have a github account click [Here](http://github.com) to register an account.

1. Enter your information
    * Enter the username and password that you're going to used and your email address that you are registering with
    * Remeber to keep track of your account so write it down somewhere so you can remember it

2. Choose Plans for beginner (It's Free)

3. Complete set up
    * Follow the direction it tell you to do by clicking complete setup (This is really opitional but it your choice if you want to do it)

4. Verify your email address
    * Log on your email and verify the account that you're about to make this insure your safey that you're using your email and not anyone else 

5. Once you finish registering your account for github you need a IDE which is a integrated development environment that stores your code locally and a place where you can type your code in while you're working. The current one that we are working with is called [ide.cs50](ide.cs50.io) click the link if you haven't already, there also other place that you can make your ide but they cost money so we're working with a free one. This ide is benefical because it a sand box that you can mess around in rather then your computer terminal where you can cause permant damage to it.

Follow the steps [here](https://github.com/hstatsep/ide50) to set up your IDECS50


> #### Whats is SSH?  
> SSH stands for Secure SHell which goes through a protocal to help someone safety access the net.

---
## Repository Setup
    git init
Initialize git in our directory (now called a repository) for version control
    -Only do it once at the beginning 
    
    git add .
adds current directories (all files that  have changed including the deleted ones and renamed)

Before anything, your need to initialize your git, create a directory that your file will be contain at by using `Mkdir < File Name >`. A directory is a library that store your information or project within such as files, documents, images, and videos. After you initialize your git you would need to `cd < file name >` to make any changes within the directory. Then you would need to do `git init` to initialize the git which make the file into the parent function of every other. This also means that you can store anything within where it's considers as the `(master)` in your code.

As you start making changes to your files start checking what you have done by using `git status` to see the changes that you're making before you're commiting any files. Saving changes or taking _snapshot_ on your work process is really important since you'll be able to track your changes over time rather then see one whole change. Another important thing is that by saving your change every so often you won't be able to lose your work unless you have auto save on. To be able to make a change you have to used `git status` to check if the file name is green before anything.

To be able to take a _snapshot_ of your code you have to set the code onstage so it can be _prepare_ to take a picture. You have to use the command `git add .` or specfics files by using `git add < file name >` to get them onstage so they can be able to save your file.

After when you add everything onto the stage by using `git add .` you have to be ready to take the picture which saving the change you have made into your file. By using the `command git commit -m "message"` your saving the changes you by. The `-m "message"` means that your are leaving a message so you can look back at the changes you have made by using `git log`.

---
## Workflow & Commands
    status
An optional yet recommended command to see which files are staged for the community (they will show up green)

    add
adding files that have been changed or modified 
    - RED (not staged)
    - GREEN (staged)
    
    commit
To commit is to modify your code and the command you use is git commit -m ""

After when you already get everything start you can mess around with what you're doing start by making a repository as you were taught in repository set up by using the command `mkdir < file name >` then jump into the folder name by using `cd < file name >` so you can start by making changes to it. Don't forget this is a new step that you'll need to learn to make a file that you can type thing in you need to use this command called `touch < file name >`. After you create your new file whatever name you call it you need a way to enter the file you can enter it by using the side bar and by double clicking or using `c9 < file name >`

When you finish making some change to your file you need to save it go ahead and save it , fine ill show you again used `git add .` to save the file and then commit by using `git commit -m "< message >`. 

Now what, after all that work and you can't present it to anybody, you actually can. Go log in your github account if you haven't already in another tab and go to the top left corner of your page and click the little green button that saids `new`. Name your repository the same name as you name the one you just had created and add a description if you want. At the bottn you'll see a check box only check it you want to make the repo there then your ide. Now this is crueial copy the first link and paste it to your ide it should look like this `git remote add origin git@github.com:<your user name>/Name.git` and after that copy the other link `git push -u origin master` and paste. After doing all that it establish a connect between your ide and github but already used `git push` when you make neww commit if you want it to be seen in github.

Also if you want to make changes to your folder name you can use `mv < current name > < new name >` but I won't go too much into command line learn it yourself. To remove a file you can used `rm -rf < file name >` it remove everything inside so becareful when you use it or it migh delete everything without asking your permission. Don't forget always do `git status` whenever you work so you can see the changes you make

At the botton there a chart of some command that I won't really go indept about so fell free to look or take a glance at it


Command | Explaination
---|---
`git init` | Initializes git in our directory which means making the folder into a parent function
`rm -rf < file name >` |  remove a file compelely
`git add .` | add a file onto the stage
`git commit -m "message"`| saves the changes you made and add a message
`git remote add origin URL`|Set the origin of the repo just in case if you used it to make other repos
`git push -u origin master`| This tells git to remember which remote repo & branch to push our changes to when we type git push in the future
`git push`|Send your code or _snapshot_ into a server
`git diff`|See the difference between your current code and you previous
`git log`|See your last commit
`git remote -v`|Tells you where git push will send your commits to (git status for your remote)
`git status`|command to see what files are staged for the commit








---
## Rolling Back Changes

Once you make any change you can't really do much about it. Actually you can where you can still travel back in time of what you have done before. You can always used `git log` and `git revert` to go back to the change you have made before but this is for when you already added something to stage or you already made a commit. To disgard any change you have just make you can use the command `git checkout --< file name >`. Also used `git diff` to check if you did it correctly read the chart if you don't know what it does.

#### Undo Edits

> To undo edits you have to first make some changes to a folder and do not add them to the stage nor commit. Do git status and your would see a chunk of words. Type the first command that was given to you and you'll be able to undo your edits

#### Undo add

> Go make changes to any file and do git add . to add them onto the stage. Then do git status and type the command onto of the green file name and you would undo the add and remove them from the stage

#### Undo commits

> What if you made a mistake and "accidentally" added a file onto the stage and commited the file. Don't worry check git status and do git reset --hard HEAD^ to undo a commit that was done by you. To undo multiple commits you can add a ~ and a number behind it to remove amount of commit you done.


