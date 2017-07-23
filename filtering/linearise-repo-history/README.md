Linearise Repository History
============================

About
-----

Removes merge-commits and all commits that link to other branches. A more details
explanation and example is provides [here][1].

Usage
-----

```sh
$ git filter-branch --parent-filter 'cut -f 2,3 -d " "'
```

[1]: https://stackoverflow.com/a/17994534/
