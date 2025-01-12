# Error
since util-linux 2.40.3, mounting glusterfs will pop up the error below
```
# mount -t glusterfs server1:/volname /mount_point
ERROR: Server name/volume name unspecified cannot proceed further..
Please specify correct format
Usage:
man 8 /usr/bin/mount.glusterfs
```

# Fix
Tested with util-linux 2.40.2 and 2.40.3
```
# patch /usr/bin/mount.glusterfs ~/mount.glusterfs.patch
patching file mount.glusterfs
```

# Fair License

Copyright 2025 Manhong Dai

Usage of the works is permitted provided that this instrument is retained with the works, so that any entity that uses the works is notified of this instrument.

DISCLAIMER: THE WORKS ARE WITHOUT WARRANTY.
