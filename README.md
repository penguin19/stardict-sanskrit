# Updating dictionary files for distribution
## Initial  setup.
* Install the latest stardict tools package (<https://sourceforge.net/projects/stardict-4/files/3.0.1/stardict-tools-3.0.1.tar.bz2/download>) in the stardict your home directory (accessible with ~ in linux).
* Clone <https://github.com/sanskrit-coders/sanskritnlpjava> in your home directory.
* Clone this repo.

With sa-vyAkaraNa/laghu-kaumudi/laghu-kaumudi.babylon as an example:
* Update the babylon file.
* Change directory to sa-vyAkaraNa.
* Run: make DICTS='laghu-kaumudi'. This will run the commands listed in sa-vyAkaraNa/makefile sequentially. All dictionaries and tars under sa-vyAkaraNa will be rebuilt as of 20160321.
* Watch out for errors and warnings.
* If you are satisfied with the output, commit and push.


# Other notes
Recipe to convert decompiled en-head dictionaries from ajita to sa-head dictionaries: ^.+\t(.+?)\.  should be replaced by \1\t
