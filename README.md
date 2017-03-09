# Docker Library PHP - additional PHP versions

This is a fork of the official Docker Library PHP image https://github.com/docker-library/php/ with additional PHP versions.

Branches:
* docker-library-master: Master branch from original Docker Library repo https://github.com/docker-library/php/ .
* master: Master branch for this repo. Will be merged with docker-library-master regularly.

## Create Docker images - example

```bash
cd 5.6/apache
docker build . -t eugenesia/php:5.6-apache
```

## Update Dockerfiles - example

For PHP >= 5.5:
```bash
./update.sh 5.5
./update.sh 5.6
./update.sh 7.0
./update.sh 7.1
```

For PHP <= 5.4:
```bash
./update-gz.sh 5.4
~~./update-gz.sh 5.3~~ (compiling PHP 5.3 fails for a number of reasons)
```

## Dev notes

Merge with upstream original repository at docker-library:

```bash
git remote add upstream git@github.com:docker-library/php.git
git fetch upstream
git checkout master
git merge upstream/master
# Check which local branch is tracking which remote branch.
git branch -vv
```

References:
* Configuring a remote for a fork: https://help.github.com/articles/configuring-a-remote-for-a-fork/
* Syncing a fork: https://help.github.com/articles/syncing-a-fork/

