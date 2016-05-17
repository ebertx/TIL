# Fix Mac ignoring renaming lowercase to uppercase

Multiple times I've had an issue where I named a directory "example" and later wanted to change it to "Example". On my MacBook, everything looked fine, but when viewing my repo on BitBucket or in production, I would notice an "example" folder and "Example" folder existing side by side.

In `.git/config`, change

```
ignorecase=false
```

to

```
ignorecase=true
```

[Source](https://www.garron.me/en/bits/git-ignorecase-rename-lowercase-uppercase.html)
