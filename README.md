![GitHub release (latest by date)](https://img.shields.io/github/v/release/FS-make-simple/mmv)
![GitHub Release Date](https://img.shields.io/github/release-date/FS-make-simple/mmv)
![GitHub repo size](https://img.shields.io/github/repo-size/FS-make-simple/mmv)
![GitHub all releases](https://img.shields.io/github/downloads/FS-make-simple/mmv/total)
![GitHub](https://img.shields.io/github/license/FS-make-simple/mmv)

# mmv

move/copy/append/link multiple files by wildcard patterns

### Description

Mmv moves (or copies, appends, or links, as specified) each source file matching a from pattern to the target name specified by the to pattern.
This multiple action is performed safely, i.e. without any unexpected deletion of files due to collisions of target names with existing filenames
or with other target names. Furthermore, before doing anything, mmv attempts to detect any errors that would result from the entire set
of actions specified and gives the user the choice of either proceeding by avoiding the offending parts or aborting. mmv does support large
files (LFS) but it does *NOT* support  sparse files (i.e. it explodes them).

### Files

* mmv{.exe}	--	The mmv program, set for -x default and slow id method.
* mmv.man	--	Printable documentation. Edit to remove _^H's to display on the screen.
* mmv.c	--	Source for mmv, compatible with Turbo C 1.5. Compile in compact model with MSDOS defined.
* mmv.1	--	Source for mmv.man. Use nroff -man -rO2.
