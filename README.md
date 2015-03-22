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
