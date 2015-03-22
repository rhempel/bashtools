# bashtools

Collection of bash scripts and templates that come in handy from time to time 

Yet another collection of `bash` compatible helper scripts and templates that
have come in handy over the years.

These tools can be used as a `git` submodule as follows:

```
git submodule add https://github.com/rhempel/bashtools.git [path]
```

The `path` is optional, if you don't specify one, then you'll get
a new subfolder called `bashtools` in your project.

If you do a `git status` now, you'll see two new files:

```
On branch master
Your branch is up-to-date with 'origin/master'.
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   .gitmodules
	new file:   bashtools

```

Add these two files to your next `git commit` and then push to your
`origin` repo.

When you clone the repo with the `bashtools` submodule, you need to 
take two extra steps:

```
git submodule init
git submodule update
```

This will retreive the state of `bashtools` when the repo containing
the `bashtools` submodule was committed - not the latest and greatest
`bashtools`.

If you actually want the latest and greatest code, just do this:

```
cd bashtools
git pull origin
```

From there you'll need to test your scripts against any changes, and then
when you're satisfied you can commit the `bashtools` folder to your actual
project repository.

For example, let's assume we've just pulled the latest `bashtools` into
the project we're working on, `git status` will show:

```
On branch master
Your branch is up-to-date with 'origin/master'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   bashtools (new commits)
```

This tells us that we need to commit the `bashtools` folder so that the
next time we clone this project, we get the correct `bashtools` files.
