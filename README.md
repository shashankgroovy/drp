drp
===

Drp is a command line tool for Dropbox to ease upload, download of files and get public URLs.

Installation
------------

```
$ wget http://goo.gl/yS0X9B
$ chmod +x main.py
```
Requirements
------------

- Python (Duh!)
- `pip install dropbox`
or [Dropbox Python SDK](https://www.dropbox.com/developers/core/sdks/python)
- `pip install click` (for CLI interface)

Command Usage
--------------

```
$ drp                                    # show help
$ drp init                               # initialize drp
$ drp [-p path] up file1 file2           # upload files
$ drp [-p path] down file1 file2         # download files
$ drp ls [path]                          # list files
$ drp tree [path]                        # show file structure
$ drp mkdir folder                       # creae a new directory
$ drp rm file                            # delete file or empty directory
$ drp share file                         # copy public URL to clipboard
$ drp info file                          # retrieve metadata for file/folder
$ drp search [-p path] query             # Search for files/folders containing the given string
```

Todos
-----

* Add search function
* Extend with parallel uploads and downloads
* Use compression for file transfer (gzip)
* Set multi-threaded transfer for large uploads/downloads

License
-------

Drp is released under the [GNU GPL License v3](http://www.gnu.org/licenses/quick-guide-gplv3.html).
