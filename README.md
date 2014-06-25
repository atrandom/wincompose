﻿WinCompose
==========

A compose key for Windows, written by Sam Hocevar.

A **compose key** allows to easily write special characters such as **é
ž à ō û ø ☺ ¤ ∅ « ♯ ⸘ Ⓚ ㊷ ♪ ♬** using short and often
very intuitive key combinations. For instance, **ö** is obtained using
<kbd>o</kbd> + <kbd>"</kbd>, and **♥** is obtained using <kbd>&lt;</kbd>
\+ <kbd>3</kbd>.

I wrote WinCompose because I found none of the alternatives (FreeCompose,
CKFW, AllChars or Unichars) to be satisfying.

Download latest: [WinCompose 0.6.9](https://github.com/samhocevar/wincompose/releases/download/v0.6.9/WinCompose-Setup-0.6.9.exe) (June 25, 2014)
-----------------------------------

Portable version: [WinCompose 0.6.9 (portable)](https://github.com/samhocevar/wincompose/releases/download/v0.6.9/WinCompose-0.6.9.zip).

Older versions are available [in the releases section](https://github.com/samhocevar/wincompose/releases/).

Quick start
-----------

After installation, WinCompose should appear in the System Tray. Press and
release the <kbd>⎄ Compose</kbd> key to initiate a compose sequence (this key
defaults to <kbd>Right Alt</kbd>); the icon should change to indicate a compose
sequence is in progress.

Then type in the keys for a compose sequence, such as <kbd>A</kbd> then
<kbd>E</kbd> for **Æ**:

![Quick Launch](/web/shot1.png)

If <kbd>Right Alt</kbd> is not suitable for you, you can change it in the settings.

Examples
--------

Compose rules are supposed to be intuitive. Here are some examples:

 - <kbd>⎄ Compose</kbd> <kbd>\`</kbd> <kbd>a</kbd> → **à**
 - <kbd>⎄ Compose</kbd> <kbd>'</kbd> <kbd>e</kbd> → **é**
 - <kbd>⎄ Compose</kbd> <kbd>^</kbd> <kbd>i</kbd> → **î**
 - <kbd>⎄ Compose</kbd> <kbd>~</kbd> <kbd>n</kbd> → **ñ**
 - <kbd>⎄ Compose</kbd> <kbd>/</kbd> <kbd>o</kbd> → **ø**
 - <kbd>⎄ Compose</kbd> <kbd>"</kbd> <kbd>u</kbd> → **ü**
 - <kbd>⎄ Compose</kbd> <kbd>o</kbd> <kbd>c</kbd> → **©**
 - <kbd>⎄ Compose</kbd> <kbd>+</kbd> <kbd>-</kbd> → **±**
 - <kbd>⎄ Compose</kbd> <kbd>:</kbd> <kbd>-</kbd> → **÷**
 - <kbd>⎄ Compose</kbd> <kbd>(</kbd> <kbd>7</kbd> <kbd>)</kbd> → **⑦**
 - <kbd>⎄ Compose</kbd> <kbd>C</kbd> <kbd>C</kbd> <kbd>C</kbd> <kbd>P</kbd> → **☭**
 - <kbd>⎄ Compose</kbd> <kbd>&lt;</kbd> <kbd>3</kbd> → **♥**

The full list of rules can be found by clicking on the WinCompose system tray
icon or using the “Show Sequences…” menu entry:

![Sequence List](/web/shot2.png)

The window allows you to filter the sequences being listed.

Features
--------

WinCompose supports the standard Compose file format. It provides more than
1600 compose rules from the [Xorg](http://www.x.org/wiki/) project and the
[dotXCompose](https://github.com/kragen/xcompose) project. You can add custom
rules by creating a file named `.XCompose` or `.XCompose.txt` in your
`%USERPROFILE%` directory.

WinCompose supports rules of more than 2 characters such as <kbd>⎄ Compose</kbd>
<kbd>(</kbd> <kbd>3</kbd> <kbd>)</kbd> for **③**.

WinCompose supports early exits. For instance, <kbd>⎄ Compose</kbd> <kbd>&</kbd> will
immediately type **&** because there is currently no rule starting with <kbd>&</kbd>.

As of now, WinCompose is fully translated in two languages: French and Greek. You can help us translate it to more languages using the Weblate project:

<a href="https://hosted.weblate.org/engage/wincompose/?utm_source=widget"><img src="https://hosted.weblate.org/widgets/wincompose-287x66-white.png" alt="Translation status" /></a>

Bugs
----

WinCompose is known to *sometimes* misbehave in the following situations:
 - When the Synergy keyboard sharing software is running.
 - When several keyboard layouts are installed on the computer and they are
   changed on the fly.

Most of these issues are actually bugs in the AutoHotKey software upon which
WinCompose is based.

Please report bugs to Sam Hocevar <sam@hocevar.net> or to the [GitHub issue
tracker](https://github.com/samhocevar/wincompose/issues).

