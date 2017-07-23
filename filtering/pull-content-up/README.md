Pull Up Content
===============

About
-----

There might be cases where you want to move content within a directory
structure up. One could use a `git rebase` or even just a `git mv`, but these
would either mean editing lots of commits by hand, or adding meaningless commit
to the history. Doing a `git filter-branch` operation can have the same effect
by modify all commits in one go.

Usage
-----

```sh
$ git filter-branch -f --prune-empty --subdirectory-filter <DIR>
```

where `<DIR>` is the directory whose content you wish to pull-up.
