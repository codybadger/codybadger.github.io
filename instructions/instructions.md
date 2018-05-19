---
layout: default
title: Instructions
---

# {{page.title}}

## Serve the pseudo-site:

* `bundle exec jekyll serve` - To begin serving while building the site

## Make sure repo is up to date:

* `git pull` - Fetch from and integrate with another repository or a local branch
* `git pull origin master` - More generally, a branch that is created from a remote branch will pull by default from that branch. So, `git pull origin master` fetches a copy of the master branch from the original repository, and merges it with the current branch you have checked out.

## Changes are done, time to add:

* `git add .` -
  * `git add -A` stages All - `git add -A` is equivalent to  `git add .; git add -u`.
  * `git add .` stages new and modified, without deleted. The important point about `git add .` is that it looks at the working tree and adds all those paths to the staged changes if they are either changed or are new and not ignored, it does not stage any `rm` actions.
  * `git add -u` stages modified and deleted, without new. `git add -u` looks at all the already tracked files and stages the changes to those files if they are different or if they have been removed. It does not add any new files, it only stages changes to already tracked files.

git add -A is a handy shortcut for doing both of those.

* `git commit "name-of-commit"` - Stores the current contents of the index in a new commit along with a log message from the user describing the changes.
* `git push` - Updates remote refs using local refs, while sending objects necessary to complete the given refs.