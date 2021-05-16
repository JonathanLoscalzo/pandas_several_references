

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

```

# 1

git remote add -f learn_pandas_petrou https://github.com/tdpetrou/Learn-Pandas
git remote add -f learn_pandas_hrojas https://bitbucket.org/hrojas/learn-pandas.git
git remote add -f pandas_exercises https://github.com/guipsamora/pandas_exercises # forked repository: https://github.com/JonathanLoscalzo/pandas_exercises.git
git remote add -f pandas-cookbook https://github.com/jvns/pandas-cookbook.git

#2
git subtree add --prefix=learn_pandas_hrojas learn_pandas_hrojas/master --squash
git subtree add --prefix=pandas_exercises pandas_exercises/master --squash
git subtree add --prefix pandas-cookbook pandas-cookbook/master --squash


```




## Subtree references
 - https://github.com/git/git/blob/master/contrib/subtree/git-subtree.txt
 - https://www.atlassian.com/git/tutorials/git-subtree
 - https://gist.github.com/SKempin/b7857a6ff6bddb05717cc17a44091202
