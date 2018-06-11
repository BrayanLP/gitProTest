# gitProTest

Practicando de manera Pro con Git

## Creating a feature branch

When starting work on a new feature, branch off from the develop branch.

```
$ git checkout -b myfeature develop
Switched to a new branch "myfeature"
```

## Incorporating a finished feature on develop

Finished features may be merged into the develop branch to definitely add them to the upcoming release:

```
$ git checkout develop
Switched to branch 'develop'

$ git merge --no-ff myfeature
Updating ea1b82a..05e9557
(Summary of changes)

$ git branch -d myfeature
Deleted branch myfeature (was 05e9557).

$ git push origin develop
```

![alt text][logo]

[logo]: https://nvie.com/img/merge-without-ff@2x.png 'Imagen Branch Develop'

## Create Tag

```
$ git tag -a 1.2 -m "message"
$ git push --tags
```
