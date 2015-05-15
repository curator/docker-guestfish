libguestfs-tools
=============

Run guestfish and other [libguestfs-tools](http://libguestfs.org) in a container.  Especially useful on platforms where compilation is impractical or unpossible (Mac OS X, Windows, etc.).

Defaults to running guestfish


"Installation"
=============
Create an alias (in your .zshrc or .bashrc or whereever appropriate):
```guestfish () { docker run -it --rm -v $PWD:/root/$PWD curator/guestfish $@ }```

Usage
=============
```guestfish --rw -a /root/$PWD/someimage.qcow2```

>You did it!

>*justinclayton*
