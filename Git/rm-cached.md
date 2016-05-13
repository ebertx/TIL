# Remove files listed in .gitignore

If you end up adding a new directory to your .gitignore, you may have a bunch of files you've already added to your repo that you now want to be ignored. It's easy to forget to add a new directory to your .gitignore, so this seems to happen a lot (at least to me).

```
git rm --cached .
git add .
git commit -m "Remove files"
```

The first line removes all of the files. The second line re-adds all of them, minus whichever new exceptions you've added to your .gitignore. 

[Source](http://stackoverflow.com/questions/13541615/how-to-remove-files-that-are-listed-in-the-gitignore-but-still-on-the-repositor)
