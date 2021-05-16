

## Commands

To updates the code of the subtrees
```
git subtree pull --prefix <local folder> <origin subtree> <branch> --squash

```

**Note**: This is very quick and painless, but the commands are slightly lengthy and hard to remember. We can make the commands shorter by adding the sub-project as a remote.

### Adding subtrees as a remote

```
git remote add -f <local folder> <repository url>
```

and then, we can add remote subtrees as: 
```
git subtree add --prefix <local folder> <remote-subtree> master --squash
```


# 1
git remote add -f learn_pandas_petrou https://github.com/tdpetrou/Learn-Pandas
git remote add -f learn_pandas_hrojas https://bitbucket.org/hrojas/learn-pandas.git
git subtree add --prefix <local folder> <remote-subtree> master --squash


```




## Subtree references
 - https://github.com/git/git/blob/master/contrib/subtree/git-subtree.txt
 - https://www.atlassian.com/git/tutorials/git-subtree
 - https://gist.github.com/SKempin/b7857a6ff6bddb05717cc17a44091202
