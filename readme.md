# bash-utils
## exif_renamer.sh
Usage: exif_renamer [input]

Possible input:
 - -h --help: displays this help
 - path: renames jpeg files found under the path so, that the photos are sorted by
 	1. "Create Date" if found in exif data of the image,
 	2. "Modification Date" or "Modify Date" else.

The new filenames indicate also the respective date and time.

If no input is specified program renames jpeg files in the current directory.
