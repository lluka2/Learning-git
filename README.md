# A repo for a git workshop with the Klepac-Ceraj Lab

Many of the git commands used in the tutorial can be found below. As you follow
along the tutorial, feel free to copy-paste to make things easier. Stuff
enclosed in `<BRACKETS>`, and in all caps should be replaced with user-specific
info

1. [Git local set-up (global config)](#config)
1. [Cloning the repo](#clone)
2. [Stage changes](#stage)
3. [Commit changes](#commit)
4. [Push changes](#push)
5. [Make a new branch](#branch)

**<a name="config"></a>Global Configurations**

[See here][1] for more info

```sh
$ git config --global user.name "<YOUR NAME>"
$ git config --global user.email <YOUR EMAIL>
```

**<a name="clone"></a>Cloning the Repo**

The repo is hosted [on github][2]

```sh
$ git clone https://github.com/kescobo/KCLabgit.git
$ cd KCLabgit
```

**<a name="stage"></a>Stage changes with `git add`**

```sh
$ git add <FILE_NAME>
```

**<a name="commit"></a>Commit changes**

```sh
$ git commit -m "<COMMIT MESSAGE>"
```

Alternatively, you can just do:

```sh
$ git commit
```

And your default shell text editor will open, allowing you to enter a commit
message. If your files are already version controlled, you can skip the "stage"
step, commiting all previously tracked files in one command using the `-a` flag:

```sh
$ git commit -am "<COMMIT MESSAGE>"
```

**<a name="push"></a>Push Changes**

If you cloned the repo, your "upstream" is already set. If you want to push to
the same repo:

```sh
$ git push
```

If you want to push somewhere else, you can set a new upstream repo:

```sh
$ git remote add <REPO_NAME> <REPO_URL>
$ git push -u <REPO_NAME> <BRANCH_NAME>
```

**<a name="branch"></a>Make a New Branch**

```sh
$ git checkout -b <BRANCH_NAME>
# Make changes
$ git commit -am "<COMMIT MESSAGE>"
$ git push -u origin <BRANCH_NAME>
```



[1]: https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup
[2]: https://github.com/kescobo/KCLabgit
