```
$ spot
 Spotlight CLI.

If a command takes a [path], the results will be restricted to that directory.

apps                      Installed applications.
attr                      Attributes that can be used with "spot <query>".
author <query> [path]     Files from author.
ext <query> [path]        Any files with that extension.
                              $ spot ext pdf ~
file <query> [path]       Find files.
                              $ spot file vimrc ~/dotfiles
group <group|gid> [path]  All files from user.
                              $ spot group $GID /etc
size <rel> <size> [path]  Find all files of a certain size in bytes.
                          Or (k)ilobytes, (m)egabytes, (g)igabytes.
                              $ spot size '>=' 1g ~
text <query> [path]       Find files containing text.
                              $ spot text 'ascii porn' ~
user <user|uid> [path]    All files from user.
                              $ spot user $UID /var

<path>                    Get all attributes for that path.
                              $ spot ~/fancy.gif
<query> [path]            Generic query. Supports any attributes from "spot attr".
                          See link at the bottom for the syntax.
                              $ spot foo
                              $ spot 'kMDItemMusicalGenre == *Metal*' /data/music

The Spotlight query syntax explained:
https://developer.apple.com/library/mac/documentation/Carbon/Conceptual/SpotlightQuery/Concepts/QueryFormat.html
```
