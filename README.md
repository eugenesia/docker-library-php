# Docker Library PHP - additional PHP versions

This is a fork of the official Docker Library PHP image https://github.com/docker-library/php/ with additional PHP versions.

Branches:
* docker-library-master: Master branch from original Docker Library repo https://github.com/docker-library/php/ .
* master: Master branch for this repo. Will be merged with docker-library-master regularly.

## Dev notes

To pull from Docker Library repo, do this:
```bash
git remote add docker-library-origin git@github.com:docker-library/php.git
git checkout docker-library-master
# Set local branch 'docker-library-master' to track 'master' branch of
# Docker Library repo remote 'docker-library-origin'.
git branch -u docker-library-origin/master docker-library-master
git pull
# Check which local branch is tracking which remote branch.
git branch -vv
```

