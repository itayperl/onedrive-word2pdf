onedrive-word2pdf
=================
This is a script to batch convert Word documents to PDF using OneDrive and Word
Online. It's fast and produces very good results.

I used it a lot with documents containing math, which LibreOffice couldn't
handle.

Dependencies
------------
* Python 2.7
* python-onedrive
* Gtk 3 and WebKit with gobject introspection
* python-gi

Installation
------------
* Configure python-onedrive according to the [instructions](https://pypi.python.org/pypi/python-onedrive/#command-line-usage). You'll have to create a LiveConnect application [here](https://account.live.com/developers/applications).
* Run `word2pdf -l`. It will display a browser window and ask you to log-in to
  OneDrive. Tick 'Keep me signed in' so you don't have to do this every time:
  the cookies will be saved.

Usage
-----
* Run `word2pdf --help` for CLI usage.

TODO: Rewrite using PhantomJS once [file download is supported](https://github.com/ariya/phantomjs/issues/10052).
