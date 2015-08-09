git-create-deploy-branch
========================

Creates and maintains a derivative branch of the current branch containing
normally gitignored files for deployment.

Any files specified on the command line will be added to the deploy branch, or
if unspecified, anything listed in the `.gitdeploy` file in the root of the
repository. If that does not exist, it will add everything in the repository.

This tool completely ignores `.gitignore` files.

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
