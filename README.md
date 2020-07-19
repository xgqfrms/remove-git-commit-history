# remove-git-commit-history

https://github.com/xgqfrms/remove-git-commit-history

## git filter-branch

https://www.cnblogs.com/xgqfrms/p/13338946.html


```sh
# $ git clone https://github.com/xgqfrms/remove-git-commit-history
$ git clone git@github.com:xgqfrms/remove-git-commit-history.git

$ cd github/remove-git-commit-history

$ git filter-branch --force --index-filter \
  "git rm --cached --ignore-unmatch tools/sensitive-data.md" \
  --prune-empty --tag-name-filter cat -- --all

# OR ???
$ git filter-branch --force --index-filter "git rm --cached --ignore-unmatch tools/sensitive-data.md" --prune-empty --tag-name-filter cat -- --all

```

## SSH !== HTTPS


https://www.cnblogs.com/xgqfrms/p/13339250.html
