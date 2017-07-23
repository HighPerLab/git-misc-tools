Move Content
============

About
-----

Move files and directories around while maintaining repository history, without
adding a meaningless commit.

Usage
-----

```sh
$ git filter-branch -f --tree-filter 'mv <SRC> <DST>' HEAD
```
