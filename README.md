# dmenu-exec-program
A simple program that works with dmenu to present the user with a list of statements that map to actual commands.

The program is written in POSIX compliant shell script and it has two key advantages:
1. it uses the already existing alias functionality to map statements to commands instead of inventing its own.
2. it allows spaces in statements ( but not the word "SPACE", since this is what the program uses to replace the spaces in the statments with ).

The program reads a config file named ".fpalias" by default in the users home directory, and builds a list of aliases.

Each line has the format of "alias,command".

Due to having problems setting "=" as a field separator, I use "," as a field separator.

The only window manager I have tested it with is i3, but you're free to try it with other window managers.

You can give me feedback on what I should add or improve, have fun :>

# Sample ".fpalias" configuration file
```
IRC client,hexchat
chromium with proxy,chromium --proxy-server="..."
audio,pavucontrol
telegram,telegram-desktop
office,libreoffice
torrent client,transmission-gtk
```
