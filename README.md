# Table of Contents



# Launch GDB to debug executable
1. Launch GDB from any directory then select the file
~~~
$ gdb
(gdb) file [relative path to file]
~~~
2. Launch GDB with file as arguement
~~~
$ gdb [relative path to file]
~~~

# Run executable
Use the command `run`.

# Pass executable args
1. After launching GDB and before running you can use the `set args` command.
~~~gdb
(gdb) set args [arg1] [arg2] [arg3] [...]
~~~
2. When using the `run` command you can pass the arguements through, but it will start running the executable.
~~~gdb
(gdb) run [arg1] [arg2] [arg3] [...]
~~~

# Set Breakpoints
1. To set a breakpoint type `break [line #]` to set a breakpoint in the file that makes the executable.

1. To set a breakpoint in a different file type `break [relative file path]:[line #]`.


# Usefull Commands while in GDB

## Clear Terminal/Command Screen
----

1. Most environments support `CTRL + L` to clear screen.
2. You can also use the command `shell clear`.

## Quit GDB
----
1. Most environments support `CTRL + D` to exit and `y` to confirm.
2. You can also use the command `quit` to quit GDB.

## Pause execution
----
To pause execution use `CTRL + C`.

## Print code around a line
----
Use the command `list [relative file path]:[line #]` to print 5 lines before and 5 lines after selected line.