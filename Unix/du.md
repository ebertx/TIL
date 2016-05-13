# Check disk usage of a folder

I already knew how to check the used and available space on each mounted drive.

```bash
df -h

Filesystem      Size  Used Avail Use% Mounted on
udev            3.9G     0  3.9G   0% /dev
tmpfs           788M  9.5M  779M   2% /run
/dev/sdb1       103G  9.4G   88G  10% /
tmpfs           3.9G   84K  3.9G   1% /dev/shm
tmpfs           5.0M  4.0K  5.0M   1% /run/lock
tmpfs           3.9G     0  3.9G   0% /sys/fs/cgroup
cgmfs           100K     0  100K   0% /run/cgmanager/fs
/dev/sda1       4.6T  1.7T  2.7T  39% /mnt/untitled
tmpfs           788M   52K  788M   1% /run/user/1000
```

TIL that to check how much space a specific directory uses, you use the `du` command. `du` by itself recursively shows the disk usage of every folder and sub-folder from the current location. The `-s` parameter gives a summary of the disk usage, `-h` makes it human readable, and supplying the target directory as the final parameter narrows the scope. So...

```bash
du -sh ~/Music
```

Would tell you how much space your Music drive takes up, resulting in something like this:

```bash
48G	Music
```

[Source](http://www.cyberciti.biz/faq/checking-directory-size-in-linux-command/)
