# Git, what it does and setting it up.

> Git is a source code which allows the users to be able to easily manage and complete grouped or multi-branch projects, let it be a group one or a an individually managed one.
 It is a very useful source code that remains very popular to this day and has been highly supported upon by its fanbase, which makes it extremely viable to this day.
It can do everything from simple individual coding to the biggest and fanciest code imaginable so no wonder why it's so versatile and widely used.

* __So the reasons to use it are fairly large and it really simplifies the coding work you would have to do.__

## So you are probably wondering: how do I, the reader, get my hands on this fine piece?

__Well I've got the answer for you!__

* Firstly you need to make yourself a GitHub account.
It is quite simple work and is completely free, so what's there to lose?
__After you have put in your account credentials you should then move on to step 2:__ 
Which isn't the repository just yet..

* _The next step is the creation of your own security token which can be done by following the tutorial [here](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)._                                      
 It's an official GitHub one so it's very easy to understand.

## Onto the third step to make your git come alive:

___The REPOSITORY___.

* The ___repository___ ![repository](https://git-scm.com/book/en/v2/images/newrepoform.png) 

can be set up on your [GitHub main page](https://github.com) by clicking the __NEW repository__ button on the left side of the page.
* After you have clicked the button it will ask you to name the Repository __where you will have to give it a very thoughtful and deep name like:__
 Sparngles...

Well maybe you should give it a more meaningful name than that but I ___loove Sparngles...___

* You may choose to give it a description but that is up to you, it isn't neccesary for the page.
* After that you will have the option to make it public or private depending on your wishes. 

`___Disclaimer: It is not recommended for starters to click any of the 3 buttons after that though. It is better to just leave those alone as you will make the later on.___`

* After that you will have the option to edit your GitHub page but first you must launch the terminal app on your computer __(It should already be installed on your PC/Laptop, but if not you can get it [here]( https://learn.microsoft.com/en-us/windows/terminal/install)).__

* After launching the app and connecting to your server: you must write a specific command line into your terminal:
```shell
> root@896cf839cf9a:/# git clone https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/{YOUR_REPO}.git      
```
#### Here you will:

> __Replace {YOUR_PERSONAL_TOKEN} with your token that you acquired from GitHub.   
  Replace {YOUR_USERNAME} with your username from your GitHub account.  
 Replace {YOUR_REPO} with the name of the repository that you named.__

## Congrats you have made your first git line of Code!!!

* Now your GitHub website will acquire you to enter some more code to create your _README.md_ file.

 _Don't worry GitHub has already provided you with it_. All you need to do is copy and paste it.

> __{Make sure you are on your repository directory when you make the file}__
* After you have successfully done all your tasks that GitHub has given you will be directed to the main page of your repository where your files and work to be done will be stored.

It should look like this:

![GH Main Page](https://github.githubassets.com/images/modules/site/home/repo-browser.png)

Don't worry why yours isn't as full as the images. Within time it will be.

### And a big congrats to you for successfully creating a GitHub server.

# Now that you have created your GitHub why don't you take a look at some common commands that may be used on a regular:

> git add (file names).. or to add all we use  __.__
 
Adds all of the changes we are making locally to be able to push it onto the server.
```shell
> root@896cf839cf9a:/# git add .
```
```shell
> root@896cf839cf9a:/# git add (filename)
 ```
* With the add command are also 2 other commands that must be used after it:
> git commit -m 'txt'  (makes the changes save)

The text usually signifies the type of update you are making and should be short and to the point.

This command basically makes you "Commit" to your changes and confirms them.

```shell
> root@896cf839cf9a:/# git commit -m 'Changes to README.md' 
```
The last of the `Three Musketeers` of the git commands is:
> git push  
(pushes the changes onto the server)
 
Very self explanatory, it pushes the changes we committed onto the main server.

```shell
> root@896cf839cf9a:/# git push
```
* And that is how to make changes from your local terminal onto your server.. __And anyone with access can do this not only you.__

### Which leads me onto the next topic which is: 
# Branching.

* A branch is a way for multiple people to work on the same project at the same time or can simply be used to test how a certain change could look.

> It is very effective at preventing major mishaps or changes to pass on to the main build of the project without major approval.     
 Of course it can be used for a million other reasons which shows  how versatile it is.
Truly an impressive advantage GitHub has on its competitors.

* Branching is as easy to do as a frozen pizza.  All you do is just write one command to create it and remember a few for ease of navigation.

The commands are the following:

> git branch [name of the branch]  (makes a new branch)

_Quite a simple and easy to remember command._

```shell
> root@896cf839cf9a:/# git branch [name]
```
  or if you wish to check your branches it is as simple as just writing:
> git branch

it just shows all available branches.
```shell
> root@896cf839cf9a:/# git branch
```

* Next is the command to `change branches`:  
_It actually resembles you checking out from your work, which I find amusing.._

>  git checkout <branchname>         
 (changes branches to the specified ones)
  
> git checkout -b <newname>   
(makes a new branch and switches to it)
```shell
> root@896cf839cf9a:/# git checkout <branch name> 
```
```shell
> root@896cf839cf9a:/# git checkout -b <new name>  
```
 * Afterwards lets say another peer/coworker adds an update to the server. Obviously you will need to apply it to your local version to use the most up to date one possible. You will need to use a specific other command:
> git fetch --all  
  (gets all new updates to the project)

`This one is quite important when working  with other people as its the  only way to guarantee that no overwriting mistakes will be made. ` 
```shell
> root@896cf839cf9a:/# git fetch --all  
``` 
* After getting a project done you are most likely going to want to unify all your different branches into one to lessen confusion

`So you would use this command:`
 >  git merge   
(merges 2 files)

`and in case a mistake was made:`
> git merge --abort  
(cancels the merge)

```shell
> root@896cf839cf9a:/# git <merge branch> <origin branch>
```
```shell
> root@896cf839cf9a:/# git merge --abort
```
* Whilst working you may stumble upon having multiple files that are from the same directory with similar contents.

> That will most likely have triggered an error command whilst merging asking you to fix it. The gist of it is that either I can take 30 lines talking about it here or you can just easily google it and use the command lines to fix it.

# Our BFF is GOOGLE!!

#### That is the basics of git.. Pretty cool I know , also very looong. During writing this non stop im kinda losing it...
