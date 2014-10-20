<p align="center">
  <img src="http://soundcloud-dl.com/soundcloud-download-logo.png" alt="Logo"/>
</p>
# Souncloud Music Downloader
## Changelog : MUST READ !
* the .scdl.cfg has been changed a few time ago before reporting any issue be sure you have the latest one in your $HOME !!

## Description

This shell script is able to download music from http://www.soundcloud.com.
It should work with OS X, any Linux OS.

## System requirements

* Unix like OS with a proper shell
* Tools we use : `sed` ; `tr` ; `echo` ; `grep` ; `cut` ; `sort` ; `uniq`.


## Required tools

* You will need `eyeD3` ; `curl`
* Only OSX : `brew`


## Instructions

### Just in case :
1. Download [this](https://github.com/lukapusic/soundcloud-dl/archive/master.zip)
2. Unzip

### Lazy Install :
1. You can use the auto installer : `./install` (Support Debian/arch/osX)

### Manual Install :
1. Place .scdl.cfg in your $HOME (and edit the path)
2. Be sure that you have all the required tools.
3. Place scdl in a folder that is in your $PATH (/usr/local/bin/ on OSX, /usr/bin/ for other distro by defaut)

### Fire :
1. Type `scdl {OPTION} -l {URL}`
* For help type `scdl -h`

## OPTIONS available
* `-l [URL]       ` Use this Url. (Necessary)
* `-o [OFFSET]    ` Begin the download with a custom offset.
* `-p [PATH]      ` Use a custom path for this time.  
* `-c             ` Script will continue if a sound as already been downloaded.
* `-r             ` Download only the repost.
* `-d             ` Debug mode.
* `-h             ` Show this help.

## Features

* Easy Installer
* Automatically detect which kind of Soundcloud's link you have provided
* Download all song of an user's page
* Download all repost of an user's page
* Download all song of a song page
* Download all song of an user's playlist page
* Download all song of an user's list of playlist page
* Download all song of a group page
* Download all song of an user's liked song
* Set tags with eyeD3 (skip the tag if eyeD3 is not installed)
* The script stop when he see one song that is already downloaded
* You can use it as a sync script as i do with my Raspberry PI, each night it launch the script with my soudncloud and if new song has been reposted it download it and stop when it encounter a song that has already been downloaded.

## License

[GPL v2](https://www.gnu.org/licenses/gpl-2.0.txt), orignal author [Luka Pusic](http://pusic.si)
