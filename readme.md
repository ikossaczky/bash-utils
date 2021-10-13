# bash-utils

## backup-btrfs
Script for performing backup of one or more btrfs filesystem.
- one backup copy is created on local machine
- second backup copy is sent to remote drive of choice (e.g. USB stick)
- a fixed number of most recent backups is kept, all older old backups are deleted both locally and on remote drive

Due to the usage of copy-on-write in btrfs, these backups are much faster and take much more memory than standard backups.
Btrfs filesystem is needed on both local PC and remote drive

## exif-rename
Usage: exif-rename [input]

Possible input:
 - -h --help: displays this help
 - path: renames jpeg files found under the path so, that the photos are sorted by
 	1. "Create Date" if found in exif data of the image,
 	2. "Modification Date" or "Modify Date" else.

The new filenames indicate also the respective date and time.

If no input is specified program renames jpeg files in the current directory.
