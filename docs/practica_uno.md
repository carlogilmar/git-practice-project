# Welcome to the first material for learn git.

##### Material writted by [@carlogilmar](http://twitter.com/carlogilmar)

As software developer I think that you need to know some basic things:

* Know and operate your SO through it own shell. I prefer use linux/unix. If you are using linux/unix, please check how to install ZSH (with oh my zsh) and FISH Shell (my favorite shell). If you want to be a programmer your best friend would be the shell.
* You need a text-edit for write code. Sublime-text, Atom and Visual Study are some of this. But I recommend VIM or EMACS.
* The final tool is GIT.


## GIT BASICS

Well, the first approach is that all of you can use the basic git commands, and learning with practice. Then you will need a more deep.
Please install git in your SO. In Ubuntu for example you need to write:

> sudo apt-get install git

In MacOs please:

> brew install git

If you are using Windows, download:

> https://git-scm.com/download/win

## Practice 1

### 1.- Create a git repository and add your username

Please open your terminal, and create a folder called first-repository. Go into your new folder, and type:

> git init

With this you will see a hidden folder called **.git** and you will get a git repository on your directory project.

Then you will need add a username and email, without this Git cannot do nothing.

> git config --global user.name "carlogilmar"
> git config --global user.email "carlo@makingdevs.com"

### 2.- See the status of git

Please type in the shell (into your folder):

> git status

If you don't have files, with this command GIT would say **"nothing for commit"**.

### 3.- Add a file and see the status

Add a simple file text called **first-text.txt** into your folder repository and add the following text:

> I love programming with git.

Please type in your shell:

> git status

And you will see that Git recognize your file.

For assing a control version to file, you need to do two steps: add the file to stage area (1), and write a reference(2).

### 4.- Adding your file to stage area.

Please add your file to stage area with this:

> git add first-step.txt

### 5.- Write a reference

Please write a short description for your file:
> git commit -m "Adding my first file on git"

**-m** is a flag for write by command line, if you don't write this, git will open your default text-edit.

If you want to add control version to a file, you have to do GIT ADD and then GIT COMMIT, both commands are very important.

With this steps, you will get a file with control version.

### ¡Congratulations!

### 6.- Please see your log description

> git log

And you will see the reference wrote, the username, the date, and a hash.

Until here we have learn the follow commands:

Init a git repository into a folder

> git init

See the git repository status

> git status

Adding a file to the control version

> git add file_name.txt

> git commit -m "A reference about the file"

### 7.- Please add another file, and add to control version. You will write a reference (commit), with git log you have to see both references.

### 8.- See a git difference

Please modify first-step.txt and write the following:

> I love programming. //Line modify
> New line.
> Other new line.
> Other new line.

You modify a file with control version. So, you can see the diffences between the current state, and the last reference added to control version.

Please type:

> git diff first-step.txt

And you going to see the diffences. You can accept this diffences or not.

### 9.- Accept the differences.

Please ADD and COMMIT the first-step.txt file, and see the reference with git log.

### 10.- Refuse a difference

Please modify first-step.txt with something. Check the differences with git diff

For this case, we don't want to add this change. Please type:

> git checkout -- first-step.txt

And see your file. You refuse the change, so Git returns to the last commited state.

Until here, we are using the following commands:

See the changes in a file:

> git diff file.txt

Refuse the change:

> git checkout -- file.txt

Save the change with control version:

> git add file.txt
> git commit -m "Adding a change on file.txt, this is my example reference"


## Exercise 1

1. See the Mkdocs Project, and create your own project.
2. Create your git repository and commit all the files.
3. Add your first markdown file called **me.md** and write about you.
4. Modify your mkdocs.yml for modify the visual part.
5. Modify your index.md
6. For every modification or adding, please commit.
7. See the log and see your commits.




