# ripdsl

Rip audio CDs using a python based DSL

## Workflow

Rip your CD using cdparanoia.
```
$ mkdir somedir && cd somedir
$ cdparanoia -B
```
This creates files `track01.wav.` etc in the directory `somedir`.

In parallel, search your CD release on discogs (e.g. by entering the ISBN) or
on jpc.de and pass the url to ripdsl, e.g.:
```
$ ripdsl https://www.discogs.com/de/Deep-Purple-Deep-Purple/release/9697637
```

This creates a file `tags.py` and lets you edit it with `$EDITOR` in order to
adjust the tags to your needs. You can also insert a url to the cover art.

Once cdparanoia is finished, you can let `ripdsl` encode the wav files and download the cover art.
