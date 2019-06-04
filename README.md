This package installs the `git build` command.  This command can be used to
create a QA build by merging feature branches into a transient candidate
branch, and pushing an appropriate tag for deployment.

Install
=======
```sh
sudo -H npm install -g @zingle/git-build
```

Use
===
```sh
# build to default "qa" target and base "master" branch, merging TECH-100
git build TECH-100

# use options to specify other targets or base branches
git build --tag=my-tag TECH-13
git build --base=my-super-branch TECH-42
```
