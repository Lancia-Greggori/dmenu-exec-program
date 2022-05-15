# dmenu-exec-program
A simple program that works with dmenu to present the user with a list of statements that map to actual commands

The program is written in POSIX compliant shell script and it has two key advantages:
1- it uses the already existing alias functionality to map statements to commands instead of inventing its own
2- it allows spaces in statements ( but not the word "SPACE", since this is what the program uses to replace the spaces in the statments with )

The only window manager I have tested it with i3, but you're free to try it with other window managers.

You can give me feedback on what I should add or improve, have fun :>
