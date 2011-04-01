Colorize
========
Colorize is an expressive interface for ANSI colored strings and terminal output. There are already a decent handful of string-coloring modules out there, but colorize is different in the way it works.

Most modules will have you use some kind of a colorizing function to return a string with the proper ANSI codes prepended. Colorize, on the other hand, lets you express the colorization inline (it's essentially a set of aliases for the original ANSI codes, plus a stack to allow nesting). So, if you wanted to color a word red, you would do something like:

	This word is #red[red].

You can also nest colorizations:

	#bold[Welcome to the #green[Green Machine] tool!]

Currently colorize supports the standard set of 8 ANSI colors (black, red, green, yellow, blue, magenta, cyan, white), along with bold, italic, underline, blink, and a special "reset" keyword.