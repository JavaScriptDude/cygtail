## cygtail (tail.exe)
*Nix Tail For Modern Windows - Binaries From Cygwin

These binaries are taken from recently updated Cygwin64 environment.

### Installation
```
cd <where_to_install>
git clone git@github.com:JavaScriptDude/cygtail.git
```

Then add your new path to your PATH Environment variables and presto, you now have tail available from commandline :)

### Usage:
```
> tail.exe --help
Usage: /cygtail/tail [OPTION]... [FILE]...
Print the last 10 lines of each FILE to standard output.
With more than one FILE, precede each with a header giving the file name.

With no FILE, or when FILE is -, read standard input.

Mandatory arguments to long options are mandatory for short options too.
  -c, --bytes=[+]NUM       output the last NUM bytes; or use -c +NUM to
                             output starting with byte NUM of each file
  -f, --follow[={name|descriptor}]
                           output appended data as the file grows;
                             an absent option argument means 'descriptor'
  -F                       same as --follow=name --retry
  -n, --lines=[+]NUM       output the last NUM lines, instead of the last 10;
                             or use -n +NUM to output starting with line NUM
      --max-unchanged-stats=N
                           with --follow=name, reopen a FILE which has not
                             changed size after N (default 5) iterations
                             to see if it has been unlinked or renamed
                             (this is the usual case of rotated log files);
                             with inotify, this option is rarely useful
      --pid=PID            with -f, terminate after process ID, PID dies
  -q, --quiet, --silent    never output headers giving file names
      --retry              keep trying to open a file if it is inaccessible
  -s, --sleep-interval=N   with -f, sleep for approximately N seconds
                             (default 1.0) between iterations;
                             with inotify and --pid=P, check process P at
                             least once every N seconds
  -v, --verbose            always output headers giving file names
  -z, --zero-terminated    line delimiter is NUL, not newline
      --help     display this help and exit
      --version  output version information and exit

NUM may have a multiplier suffix:
b 512, kB 1000, K 1024, MB 1000*1000, M 1024*1024,
GB 1000*1000*1000, G 1024*1024*1024, and so on for T, P, E, Z, Y.

With --follow (-f), tail defaults to following the file descriptor, which
means that even if a tail'ed file is renamed, tail will continue to track
its end.  This default behavior is not desirable when you really want to
track the actual name of the file, not the file descriptor (e.g., log
rotation).  Use --follow=name in that case.  That causes tail to track the
named file in a way that accommodates renaming, removal and creation.

GNU coreutils online help: <http://www.gnu.org/software/coreutils/>
Report tail translation bugs to <http://translationproject.org/team/>
Full documentation at: <http://www.gnu.org/software/coreutils/tail>
or available locally via: info '(coreutils) tail invocation'
```



### Checksums and virus scans
NOTE: Please confirm your checksums yourself before running any executables downloaded. Virus Total is an excellent resource for convirming individual binaries / zips etc. Below I have put the output of my [vtscan tool](https://github.com/JavaScriptDude/vtscan) which uses the Virus Total Python API.

Checksum's / Virus Total Permalinks and Scan summary for binaries:

```
/cygtail$ vtscan --nogui tail.exe 

.: Details :.
- md5: 16c3c28ca5a8f511c83769ce16ffc08d
- sha1: 5f93550a82daeaa07346f113b8a7bbba0a54d343
- sha256: 090d4921ca526fd4e1ac554126b03b8b41ec7f0b6710b5b35eb1d1d79e3b3d75
- Permalink: https://www.virustotal.com/gui/file/090d4921ca526fd4e1ac554126b03b8b41ec7f0b6710b5b35eb1d1d79e3b3d75/detection/f-090d4921ca526fd4e1ac554126b03b8b41ec7f0b6710b5b35eb1d1d79e3b3d75-1647787655

.: File :.
- File: tail.exe
- Path: /dpool/other/vm/insec-share/_1/cygtail

.: Virus Total Summary :.
- Detections: 0 out of 68 (100% pass)
```

```
/cygtail$ vtscan --nogui cygiconv-2.dll 

.: Details :.
- md5: 0b78ffe4ca2aecd20c5d4a516fb9d580
- sha1: 1fe1eb8104773c41ece210dc9604e3193b6f3893
- sha256: 60cfc666e239b063e596d91fb42d85d093a28eb0ded94a36939b03480eb9cbb5
- Permalink: https://www.virustotal.com/gui/file/60cfc666e239b063e596d91fb42d85d093a28eb0ded94a36939b03480eb9cbb5/detection/f-60cfc666e239b063e596d91fb42d85d093a28eb0ded94a36939b03480eb9cbb5-1650077627

.: File :.
- File: cygiconv-2.dll
- Path: ./cygtail

.: Virus Total Summary :.
- Detections: 0 out of 68 (100% pass)
````

```
/cygtail$ vtscan --nogui cygintl-8.dll 

.: Details :.
- md5: a26a93fe68c40b1f00f65545f50d9017
- sha1: ecbae6bdf43ace13a779f45377bd2e445d61f616
- sha256: 65c392b40a81be8793b0cc2e8052e25c93c1f305254e0e414ed3b0d8b7083714
- Permalink: https://www.virustotal.com/gui/file/65c392b40a81be8793b0cc2e8052e25c93c1f305254e0e414ed3b0d8b7083714/detection/f-65c392b40a81be8793b0cc2e8052e25c93c1f305254e0e414ed3b0d8b7083714-1650077648

.: File :.
- File: cygintl-8.dll
- Path: ./cygtail

.: Virus Total Summary :.
- Detections: 0 out of 68 (100% pass)
```

```
/cygtail$ vtscan --nogui cygwin1.dll 

.: Details :.
- md5: b3613d429aaa621b903c2b37b2fabc83
- sha1: 35fdd7e3ab7b4b36e874fc4e0df22d4feaa33500
- sha256: af1387eaf1b07d392a746d564b9b7a2dda6ee26576892da59a99132e26750fd7
- Permalink: https://www.virustotal.com/gui/file/af1387eaf1b07d392a746d564b9b7a2dda6ee26576892da59a99132e26750fd7/detection/f-af1387eaf1b07d392a746d564b9b7a2dda6ee26576892da59a99132e26750fd7-1649681172

.: File :.
- File: cygwin1.dll
- Path: ./cygtail

.: Virus Total Summary :.
- Detections: 0 out of 67 (100% pass)
```


