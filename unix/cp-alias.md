# Certain distros will alias commands like `cp` to `cp -i` in the bashrc
In order to prevent new users from blowing away files without knowing it, `cp` will be aliased to `cp -i` forcing the user to approve overwrite of files on copy. There are a few ways to get around this:

* Call the cp program using its full path: `/bin/cp`
* Call it escaped: `\cp`
* Call it using command: `command cp`
* Use `yes`: `yes | cp -rf /zz/* /xx`
