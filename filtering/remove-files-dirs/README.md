Remove Files and Directories
============================

About
-----

The following script, `remove-files-dirs.sh`, removes all files and directories
*except* those listed in the whitelist file.

Usage
-----

```sh
$ git filter-branch --prune-empty --index-filter \
  'remove-files-dirs.sh whitelist.txt' -- --all
```

Where `whitelist.txt` is of the format:

```txt
relative/path/to/file/or/dir/within/repo
```

**NOTE:** You may need to add the `-f` flag to override an previous reflog
entries/backups.
