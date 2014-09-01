# README

This repository offers N3/Turle syntax highlighting for GNOME gedit.

## Installation
Tested with Ubuntu 14.04.

``` bash
# check if mime types "text/n3" and "text/turtle" are correcty registered
$ xdg-mime query filetype path/to/somefile.ttl 
text/plain
# .. same for n3

# install mime type if needed
$ wget -P /tmp https://raw.githubusercontent.com/rmuller/turtle_gedit/master/n3.lang && xdg-mime install --novendor /tmp/n3.lang

# check again
$ xdg-mime query filetype path/to/somefile.ttl
text/turtle

# Okay, no add syntax highlighting file for gedit
$ sudo wget -P /usr/share/gtksourceview-3.0/language-specs/ https://raw.githubusercontent.com/rmuller/turtle_gedit/master/n3.lang
```

Written by Ronald Muller at 2014-08-24.
[![Ohloh profile for ronaldmuller](https://www.ohloh.net/accounts/224392/widgets/account_tiny.gif)](https://www.ohloh.net/accounts/224392?ref=Tiny)
