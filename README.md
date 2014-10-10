
Deprecated
==========

Check out the [Thyme](http://thymerb.com/) project by @hughbien with my [Mac OS X Status Bar Integration](https://github.com/dtinth/thyme_osx_ui) instead.


pmd
====

My simple Pomodoro timer for Mac OS X, command line based.

<p style="text-align:center"><img src="http://i.imgur.com/Kk7CY.png" alt="pmd!!!"></p>

Installation
------------
Please install:

* MacRuby
* Growl and growlnotify

Then clone this repository and add this to your `~/.bash_profile`:

    alias pmd=/path/to/your/pmd/pmd

Usage
-----

Run:

    pmd start

You will see a countdown timer at the top right corner of your screen. When it count to zero, you will see a Growl notification.

Configure Growl to make it emit sound.



Hooks
-----

`pmd` will also run these scripts, if they exist:

| Filename | Event |
| -------- | ----- |
| `~/.pmd/hooks/start` | When a Pomodoro is started. |
| `~/.pmd/hooks/finish` | When a Pomodoro is finished. |
| `~/.pmd/hooks/void` | When a Pomodoro is void. |



Checking the Remaining Time
---------------------------

Other scripts can check the remaining time by connecting to UNIX domain socket `/tmp/pomodoro.sock`.

For example,

    nc -U /tmp/pomodoro.sock



