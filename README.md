Souncloud music downloader
==============

Description
--------------
This shell script is able to download music from http://www.soundcloud.com.
It should work with OS X, any Linux OS.

System requirements
--------------
* Unix like OS with a proper shell
* Tools wich are preinstalled on linux (I don't know  for OS X) : `sed` ; `tail` ; `tr` ; `echo` ; `grep` ; `head` ; `cut` ; `sort` ; `uniq`.


Required tools
--------------
* You will need `eyeD3` ; `curl` ; `recode`
* The installer install all the required tools.


Instructions
--------------
* Download as ZIP ( check the button at the left of the page)
* Unzip
* You can use the auto installer : `./install` (Support Debian/arch/MacOS X)
* Type `scdl {URL}`


Features
--------------
* Easy Installer
* Autodetect wich kind of Soundcloud's link it is
* Download all song of an user's page
* Download all song of a song page
* Download all song of an user's playlist page
* Download all song of an user's list of playlist page
* Download all song of a group page
* Download all song of an user's liked song
* Set tags with eyeD3 (skip the tag if eyeD3 is not installed)
* The script stop when he see one song that have already been downloaded
* You can use it as a sync script as i do with my Raspberry PI, each night it launch the script with my soudncloud and if new song has been reposted it download it and stop when it encounter a song that has already been downloaded.


More information
--------------
The script cannot handle letters like `û` cause to recode. But if i remove it, instead of `&` you will have `&amp;` (the html code of `&`) and as i think there is more `&` than `û` i prefer to let it...


License
--------------
[GPL v2](https://www.gnu.org/licenses/gpl-2.0.txt), orignal author [Luka Pusic](http://pusic.si)
