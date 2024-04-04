# C Scripts

A couple of scripts I put together for quick C testing stuff.
I use these on MacOS but they should work anywhere with a POSIX shell.

## mkc

`mkc` creates a C source file with basic boilerplate in there.
It literally just includes stdio.h and creates a main function that returns 0.

#### Usage

```Bash
mkc <new file>
```

`mkc` will append a .c file extension to the new filename if its not supplied.

## crumb

`crumb` executes a C source file.
I used to use TCC on Linux for this purpose, but I was too dumb to get it to compile on MacOS so this was my solution.
It literally just compiles a C source file, executes a.out, and then deletes the resultant executable.
This gives the appearance of executing a C file as an interpreted script, even though it's not.
As for the name, it was originally called `crun`, but that was close to crumb so I thought it would be a fun name.

#### Usage

```Bash
crumb <source file>
```
