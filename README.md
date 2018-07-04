# ripdsl

Rip audio CDs using a python based DSL

## Workflow

Rip your CD using cdparanoia
```
$ mkdir somedir && cd somedir
$ cdparanoia -B
```

In parallel, search your CD release on github and pass it to ripdsl:
```
$ ripdsl http://discogsurl...
```

This throws you into your `$EDITOR` and you can adjust the tags to your needs. If you exit the editor you are asked whether the files shall be encoded or not. You answer should depend on whether cdparanoia is still running or not.

