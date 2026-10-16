# The sort Command

## Summary 
The `sort` command sorts or merges records (lines) of text and binary files. 

## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

Note: The sort utility sorts text and binary files by lines. Comparisons are based on one or more sort keys extracted from each line of input, and are performed lexicographically, according to the current locale's collating rules and the specified command-line options that can tune the actual sorting behavior. By default, if the keys are not given, sort uses entire lines for comparison. 

## Possible Flags

### `-R, --random-sort, --sort=random`
The `-R` flag sorts by random order. 

### `-r, --reverse`
The `-r` flag sorts in reverse order.

### `-n`
The `-n` flag sorts numbers correctly.

### `-k`
The `-k` flag sorts by a specific column.

### `-u`
The `-u` flag removes duplicate lines.

### `-c, --check, -C`
The `-c` flag checks that the single input file is sorted. If the file is not sorted, sort produces the appropriate error messages and exits with code 1, otherwise returns 0. If -C or --check=silent is specified, sort produces no output. This is a "silent" version of -c.

### `-m, --merge`
The `-m` flag merges only. The input files are assumed to be pre-sorted. If they are not sorted the output order is undefined.

### `-o output, --output=output`
The`-o` flag prints the output to the output file instead of the standard output.

### `-S size, --buffer-size=size`
The`-S` flag denotes the maximum size of the memory buffer. Size modifiers %,b,K,M,G,T,P,E,Z,Y can be used. If a memory limit is not explicitly specified, sort takes up to about 90% of available memory. If the file size is too big to fit into the memory buffer, the temporary disk files are used to perform the sorting. 

## Output
The `sort` command has many different kinds of outputs as described below:

## Examples 
* If you want to see hidden files in a nice list format run $ `ls -la ~`. The `~` would indicate your home folder.
* To get a the contents of an entire directory structure starting at a parent folder: $ `ls -alRt`. If you'd like, you can use a redirect, such as `>` to send the output to a text file. Here's an example: $ `ls -alRt ~/Desktop > ~/Desktop/report.txt`

Go back to the [main list of commands](index.md)
