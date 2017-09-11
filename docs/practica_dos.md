# Linking with remote repository

Now, you know the basic commands:

> git init
> git status
> git log
> git add
> git diff
> git checkout --
> git commit

It's time for show you the git areas:

1. Working Directory
2. Stage
3. Local Repository
4. Remote Repository

When you are using a git repository, you are on the first area: **Working Directory**.

When you ADD a file, you are send this file from **Working Directory** to **Stage Area**.

When you COMMIT this file, you are sending to **Local Repository**.

The **Local repository** is the place where you are saving your changes with control version.

Additional, you can add a **Remote Repository**, it's very useful, especially when you are working in team. First you need a platform like Github, Gogs, Gitlab, or BitBucket.

Please explore some of these platforms.

### Linking with Github

You need a Github Account. ¡It's free!

For use this service, you need to link your SSH Key.

You have to generate your own SSH Key.

Github help you to generate:

Windows Users:

> https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/#platform-windows

Mac Os Users:

> https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/#platform-mac

Linux Users:

> https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/#platform-linux


You will have a SSH Key like this:

> ssh-rsa AAAAB3refgerC1yc2EAAAADAQABAAACAQDSeM4metgrewgfZeDqAR3yt5S
> xGtHP/EyeXPZe++oGaWlfHPW6iZ0BBPAh18s2Q7rqdNq9RVQeWgcLWXhxvqOZjzNEtU
> 1DaLM+/tTdo2NLc0nptLH9er4vOKpjPXr2MNee3MrkovoO++oAoIB26c+NdNmg9FahJ
> BTj5/KGIk175VGs5Myk4+FCaObkR8FZj7je4InfIPMNKAg3twStr9Q/zzjuziQs8yBw
> HWDhRKyEvLw7K5VS+/KTq9dGy+KZjtXOIHVDuG7eK24nsE1q4jt3wNBMyd4mmCPlxOw
> Q8DBILwbVst9+4XDMbs6EzIq9OGN+oRkkQDdCyctFVifx3yMJxO4vq65rsLg08Lo/9E
> QDcTX4EUnx7Edzk47CtpAUArvkym1NzmDAUq9PJOACwiOOc0CjrLwQrAmq+lFkdRlxo
> yyS4pXHFr5Bfwff7Zw69ZcVq0tv0mBaKndNCrZfnfED5l+X9v5CP2bLfre3b7r6Nn/qt
> fRs57qQ/91veJT2IN3Fm8og9qs/RcpYTVdXeU4eJ9IqQnKJGKPtL6pk/97ZtLk2/LC0e
> fs39DIqpBQwbdi1PL1UensNd/dHBO6ezQrC6dyxgtahBIXKkOLmo8sI5zF8X25HVAVFm
> wruOkpb+kG5uZdQ2OACHJbys4QShg6NiFlJ+DyakbI6xOUjXTcf3cT9e5YQ
> == carlogilmar12@gmail.com

Please go to your Github Account, go to **Settings/SSH keys** and add your key.


### Adding your own remote repository

In your Github account, please create a **new public repository** called **first-commits**.

You will see that Github give you a url by HTTPS or by SSH.

SSH Link

> git@github.com:carlogilmar/First-Commits.git

HTTPS Link

> https://github.com/carlogilmar/First-Commits.git

This link is your remote repository, and you have to add in your local repository.

Now, go to your local repository in your computer.

Add with this:

> git remote add origin link-to-your-own-repository

Example:

> git remote add origin git@github.com:carlogilmar/First-Commits.git

If you add your remote repository, please write:

> git remote -v

And then you have to see some like this:

> origin  git@github.com:carlogilmar/git-practice-project.git (fetch)

> origin  git@github.com:carlogilmar/git-practice-project.git (push)

It's done.

## Basic Commands

### Push

You have your local repository, with commits added, and linked to remote repository.

If you want to copy your version control history in your remote repository you have to push your history.

> git push origin master

**Origin** is the link to your remote repository. And **master** is your current branch or history.

### Fetch

With this command you can update the information of the current repository

> git fetch

### Pull

In some cases you can have more commits in your remote repository, but when you want to work, you need the lastest version.

> git pull origin master

With this command you will download the lastest changes in your remote repository.


### Exercise 2

1. Create a new remote repository in github
2. Push your project created in Exercise 1













































