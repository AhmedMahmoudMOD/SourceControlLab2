# SourceControlLab2



### Modifying & Merging branch with main

![Modifiing Test Branch](screens/testcheck.png)

![Merging with Main](screens/mergecheck.png)

### Removing Branches Locally

To remove a branch locally, use the following commands:

**Sof**

```bash
git branch -d branchName
```
**Hard**

```bash
git branch -D branchName
```

### Removing Branches Remotly

To remove a branch remotly, use the following command:

```bash
git push origin -d branchName
```


### Creating Annotated Tags and Pushing remotly

![Annotated Tags](screens/tagcheck.png)

### How to List Tags Locally

```bash
git tag
```


### How to Delete Tags Locally and Remotely

Locally

```bash
git tag -d tagNname
```


Remotely

```bash
git push --delete origin tagName
```

## What is Git Rebase?

Git rebase is a command in the Git version control system that allows you to move or combine a sequence of commits to a new base commit. It is a way to rewrite the commit history of a branch, making it appear as if the changes were made on top of a different commit.

When you perform a git rebase, Git will:

1.Identify the common ancestor of the branch you are rebasing and the branch you are rebasing onto.
2.Extract the changes introduced in your branch, one commit at a time.
3.Apply these changes on top of the target branch's tip.

### Example

# Assuming you are on your feature branch
```bash 
git checkout feature-branch
```

# Start the rebase onto the target branch (main)
```bash
git rebase main
```



![GitHub Logo](https://cdn4.iconfinder.com/data/icons/iconsimple-logotypes/512/github-512.png)
