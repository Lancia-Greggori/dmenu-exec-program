# dmenu-exec-program
A simple program that works with dmenu to present the user with a list of statements/aliases that map to commands.

The program is written in POSIX compliant shell script and it has two key advantages:
1. it uses the already existing alias functionality of the shell to map statements to commands instead of inventing its own.
2. it allows spaces in statements ( but not the word "SPACE", since this is what the program uses to replace the spaces in the statments with ).

The program reads a config file named ".fpalias" by default in the users home directory, and builds a list of aliases.

Each line of the configuration file has the format of "alias,command".

Due to having problems setting "=" as a field separator, The program uses "," as a field separator.

The window managers that have been tested with include: i3,dwm

You can give me feedback on what I should add or improve, have fun :>

# For dwm users: Why use this program over the default dmenu behaviour that dwm provides?
The problem with the default dmenu behaviour used in dwm is that it provides the user with all the available commands in $PATH, most of which are meant to be executed only in the a terminal environment.
With dmenu-exec-program, you can easily specifiy a list of programs to show that you know you are going to use.

# Sample ".fpalias" configuration file
```
IRC client,hexchat
chromium with proxy,chromium --proxy-server="..."
audio,pavucontrol
telegram,telegram-desktop
office,libreoffice
torrent client,transmission-gtk
```
