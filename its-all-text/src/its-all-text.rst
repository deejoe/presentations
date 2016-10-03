:title: It's *All* Text
:css: iat-style.css


----

It's All Text
-------------

---- 

.. note: A brief preview of an idea we'll expand on later, bears repeating because it's the essence of the course.

First: 

In the most simple terms, the essence of free software and free culture is the **freedom to fork**, which is to say, to take a work, make a copy of it, and work on it as if it were your own.

.. note: and to make or improve works with the intention of allowing others also to fork

.. note: This broadens what one can do with any given work, and it broadens who can do it.

---- 

The question is:
----------------

What is the form of that work?
-----------------------------------------------

---- 

**The question is:**

**What is the form of that work?**

For software in particular, it's almost always all text.
---------------------------------------------------------

---- 

So, what are we talking about?
------------------------------

---- 

So, what are we talking about?
------------------------------

- code
- configuration
- communication
- documentation
- (some) protocols
- (some) data

---- 

Code
----

Visual programming is rare, but it exists:

- Scratch
- Piet

Usually, though, not just text, but English text with no diacritics or accents

- ASCII
- Unicode

non-Roman alphabets:

- Qalb

---- 

Configuration
-------------

- dotfiles
- ini files
- plists

---- 

Documentation
-------------

- "plain" text (see Unicode)
- various forms of markup
- reStructuredText
- Markdown
- HTML
- XML
- TeX
- YAML
- JSON

---- 

(some) Protocols
----------------

- SMTP
- HTTP
- SQL
- IRC

---- 

(some) Data
-----------

- markup (see above)
- CSV
- PDB v. mmCIF

.. note: A demonstration of PyMOL in action could be slotted in here.

---- 

Communication
-------------

.. note: This is perhaps the weakest.  f2f meetings and discussion, voice calls, video calls, these allow an immediacy that text does not.  However, they are much harder to record and use for posterity's sake.


*Subscribe to my YouTube channel!*


Video can be tedious to make, search, index, sit through, annotate, edit.

(maybe difficulty in editing is its one true advantage)

picture == 1K words ?

.. note:: They say a picture is worth a thousand words, but how many pictures does it take, for instance, to depict a novel?  War and Peace miniseries 6 x 60-80 m at 24 fps? That's a lot of pictures (and audio, too!)

---- 

How do we work with all this text?
----------------------------------

---- 

How do we work with all this text?
----------------------------------

**command line interface (CLI)**

.. note: what manipulates the data, or emits and digests the protocols?

---- 

Command-line interface
----------------------

A CLI is a *character addressable interface*

Sometimes, but often not, linear, as such.

Also known as:

- Console
- terminal

(compare with GUI)

.. note: contrast with GUI, a graphical user interface, 

.. note: terminals are graphical, just character rather than pixel oriented

----

Why Linux/Unix CLI?
-------------------

Unix paradigm has *survived and adapted* for 45 years.

*Consistent, constant, stable and widespread* way of interacting with the
computer.

*Efficient and precise.* You can issue the commands to the computer, you can
record it exactly, you can convey to someone else exactly.

---- 

Tools for text in a console
---------------------------

- Editors
- Pagers
- Interpreters
- Compilers
- servers and clients (see protocols above)

---- 

Editors/IDEs
------------

  - vi/vim
  - emacs
  - joe
  - nano
  - pico

Non-console
===========

  - IDLE
  - Jupyter/iPython
  - Notepad++
  - TextMate
  - Atom

---- 

Pagers
------

 - pg
 - more
 - less

---- 

Interpreters
------------

REPLs 
=====

  - Lisp et al
  - BASIC 
  - Forth 
  - Python
  - Ruby 
  - Lua
  - R
  - sqlite3
  - mysql
  - bash et al

---- 

Compilers
=========
 
 - FORTRAN 
 - COBOL 
 - C/C++
 - Java(ish)
 - Haskell 
 - Go
 - Rust
 - Swift

---- 

Servers and clients
===================

 (see protocols above)

 - mail 

  - mutt
  - elm 
  - pine
  - mh 
  - bsd-mailx

 - browser 

  - lynx 
  - w3m 
  - links

 - IRC 

  - weechat 
  - irssi
 
---- 

Now, for some basics
--------------------

----


Finding the terminal
--------------------

  * In Sugar: List view (Ctrl-2) -> choose the start next to Terminal activity

  * Generic Linux virtual terminal: Ctrl-Alt-Fn usually for n=1..6. Switch
    amongst VTs with Alt-Fn. Alt-F7 back to X (the GUI).

  * Terminal on MacOS

  * Cygwin, gitbash, or babun (Win)

  * Remote terminal via ssh, PuTTY (Win)

  * Termux (Android >=5)

---- 

Navigation commands
-------------------

  * pwd -- print working directory -- where am I?

  * cd -- change directory -- I want to go somewhere else?

  * ls -- list -- what's here?

---- 

Pagers
------

  * more -- run-of-the-mill paging, hit space to continue

  * less -- advanced pager with ability to backup (b), doesn't fall off until explicit quit (q)

  * pg -- a two-letter command, of course

---- 

Documentation
-------------

  * man ls

  * apropos rename

---- 

Composing pipelines
-------------------

The simplest programs: pipelines

  * ls -al | less

        STDOUT STDIN STDERR

The pipe character '|' is used to send the output of the preceding command into
the following command. Simple programs aka "one-liners".

Several commands can be strung together.

---- 

Several commands can be strung together.
----------------------------------------


.. code:: bash

 find . -maxdepth 1 -type d  -name "*_files" -print0 | \
 xargs -0 -n1 -i basename {} _files | \
 xargs  -n1 -i echo mkdir web-saved/{} \; \
 mv {}_files web-saved/{} \; mv {}?* web-saved/{} > web-saved/files_files2.sh

---- 

Filtering
---------

  * grep 

.. code:: bash

 $ /usr/share/dict/words | grep [A-Z] | less


Simple regular expressions & globs
==================================

  - ^ start 
  - $ end 


  - ? single character 
  - \* glob of characters

---- 

Making changes
--------------

Line and history editing
========================

  * history -- show commands you've issued

  * Use up and down arrows to move around history

  * Use tab completion to save typing

  * ctrl-a to beginning of line, ctrl-e to end of line

      * !n -- nth from history,

      * !! -- previous from history

      * !* -- 1st token from previous

      * !$ -- all but 1st from previous

      * ^f^b^ -- sub b for f in previous

---- 

Making changes: Retail
----------------------

Text editors
============

  * examples: 

   - nano/pico 
   - vi 
   - emacs

  * survival commands: (how to exit) 

   - ctrl-x 
   - Esc Esc Esc :q!
   - Ctrl-x Ctrl-c

---- 

Redirection
-----------

to create or overwrite a file use >

.. code:: bash 

    echo foo > bar; cat bar

to create or add to a file use >>

.. code:: bash

    echo quux >> bar; cat bar

---- 

Take command
------------
Processes and job control
=========================

See what's going on

.. code:: bash

  * ps -- list processes 

  * top -- show and compare resource usage
 
  * jobs -- show jobs and their state

---- 

Take command
------------
Processes and job control
=========================

Change what's going on

  * ctrl-c -- kill (permanent)

  * ctrl-z -- suspend (temporary)

  * fg -- foreground

  * bg -- background

  * nice -- lower priority

  * time -- how long?

  * kill -- end a process

example -- "Help, firefox is out of control!"

---- 

Making changes: Wholesale
-------------------------

Whole files & directories
=========================

  * cp -- copy

  * rm -- remove -- delete CAUTION NO RECOVERY GONE FOR GOOD

  * mv -- move -- also rename

---- 

Usage Examples:

  * cp a way to make a backup file, say, of /etc/apt/sources.list

  * rm the editor's backup files eg foo~

  * mv as a way to rename image files, say, a cryptically named image file

---- 

Querying system state
---------------------

hardware
========

"extended" ls commands

  * dmesg -- display kernel mesages

  * lsmod -- kernel modules

  * lspci -- pci bus devices

  * lsusb -- usb devices

  * lshal -- hardware access layer

  * lshw -- hardware

---- 

Querying system state
---------------------
installed software (Debian & Ubuntu)
====================================

  * dpkg -l | less -- show all packages

  * dpkg -L nano | less -- show files in a package

  * dpkg -S /usr/bin/nano -- this file belongs to which package?

  * apt-cache search foo

  * apt-get install foo

---- 

Querying system state
---------------------

installed software 
===================
(Redhat, Fedora, SoaS, et al)
=============================

  * rpm -qa -- show all packages

  * rpm -ql nano | less -- show files in a package

  * rpm -qf /usr/bin/nano -- this file belongs to which package?

  * yum search foo

  * yum install foo

  * dnf

---- 

Filesystem hierarchy and status
-------------------------------

LSB /bin, /sbin, /etc, /home, /lib, /usr/bin, /usr/sbin, /usr/lib ...

System state

  * df -- disk free

  * du -- disk usage

  * netstat -- network status

  * less /proc/cpuinfo

  * less /proc/meminfo

  * ifconfig

  * ls /var/log

  * ls /etc

---- 

Environment variables
---------------------

  * echo $HOME; echo $PATH -- show two most common

  * env -- show all environment variables

  * set FOO=bar; echo $FOO

---- 

Further topics
-------------- 

  * advanced grep (context, case), wc, with lsmod and ps

  * less -N  -- numbering

  * find foo -name "bar*" | xargs -n1 -i echo {} \;

  * chown newuser:newuser foo changing ownership

  * chmod go+r foo change access mode (permissions)

  * rsync -- convergent synchronization (local or over net)

  * scp -- remote (secure) copying

  * ssh -- remote login

  * screen & tmux -- detachable & re-attachable cli session

  * others: lynx w3m wget curl links -- CL web tools

  * others: head tail split cut -- slicing and dicing text

  * alternate shells: csh, tcsh, ksh, zsh, ash, dash

