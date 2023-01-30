# VPSUtils
Utility for Linux which adds simple commands for gaming server starting, restarting and stopping (installed *‚screen'* is required). VPSUtils also brings a feature of **auto server restart** after crash or other server failure (using watch).

## Installation:
Put files into /usr/bin directory and set their chmod to 755.

## Configuration:
Install ’screen’ (if not installed):
```sudo apt-get install screen```
or:
```sudo yum install screen```

VPSUtils by default is using user directory at */home/[username]/[servername]/Server.bin*

Server binary file should be always named as **Server.bin**.

## Usage:

Log into account, from which the server should be running.

```start [dir] [options]``` eg. start myserver -a

```restart [dir] [options]``` eg. restart myserver -off

```stop [dir]``` eg. stop myserver

#### Options:
+ -a    - enable Autorestarter
+ -d    - enable Discord Echo (not included in this release)
+ -ad   - enable Autorestarter and Discord Echo
+ -off  - disable Autorestarter and Discord Echo
Default: -ad

