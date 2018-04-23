# gnu-parallel
Experiments with the powerful command line tool GNU parallel 

## Straight from the docs
GNU parallel is a shell tool for executing jobs in parallel using one or more computers. A job can be a
single command or a small script that has to be run for each of the lines in the input. The typical
input is a list of files, a list of hosts, a list of users, a list of URLs, or a list of tables. A job
can also be a command that reads from a pipe. GNU parallel can then split the input into blocks and pipe
a block into each command in parallel.

If you use xargs and tee today you will find GNU parallel very easy to use as GNU parallel is written to
have the same options as xargs. If you write loops in shell, you will find GNU parallel may be able to
replace most of the loops and make them run faster by running several jobs in parallel.

GNU parallel makes sure output from the commands is the same output as you would get had you run the
commands sequentially. This makes it possible to use output from GNU parallel as input for other
programs.

For each line of input GNU parallel will execute command with the line as arguments. If no command is
given, the line of input is executed. Several lines will be run in parallel. GNU parallel can often be
used as a substitute for xargs or cat | bash.
