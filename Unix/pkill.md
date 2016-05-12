# Kill a process by name

This is a simple one:

```bash
pkill <process_name>
# for example:
pkill firefox
```

I mention this only because previously I had been using: `kill -9 $(pidof firefox)`, which is obviously a lot more verbose.

[Source](http://man.he.net/?topic=pkill&section=all)
