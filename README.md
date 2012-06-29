pmd
====

My simple Pomodoro timer for Mac OS X, command line based.

<p style="text-align:center"><img src="http://i.imgur.com/Kk7CY.png" alt="pmd!!!"></p>

Installation
-------------
Please install:

* MacRuby
* Growl and growlnotify

Then clone this repository and add this to your `~/.bash_profile`:

    alias pmd=/path/to/your/pmd/pmd

Usage
--------

Run:

    pmd start

You will see a countdown timer at the top right corner of your screen. When it count to zero, you will see a Growl notification.

Configure Growl to make it emit sound.