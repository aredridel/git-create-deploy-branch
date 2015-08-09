git-create-deploy-branch
========================

Creates and maintains a derivative branch of the current branch containing
normally gitignored files for deployment.

Use
-----

```shell
git checkout master
git create-deploy-branch
git show deploy/master # Just to see
git push deployhost deploy/master
```

or

```shell
git checkout master
git create-deploy-branch public
git show deploy/master # Just to see
git push deployhost deploy/master
```
