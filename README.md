# AVGTIME

`avgtime` is a bash script to run a command several times and compute the mean time of execution.

It internally uses the GNU `time` command, and display the "real" time (which is the actual time you spend waiting for your command to finish).

> :warning: this program assume that the `time` executable is in /usr/bin/time

## How to use

This is fairly simple:

```bash
$ avgtime make test # default is 10 iterations of the command
...
Mean of 10 executions of `make test`:
10.435 seconds
```

```bash
$ avgtime -n 3 make test # explicity run 3 iterations
...
Mean of 3 executions of `make test`:
11.398 seconds
```

## How to install

1. Copy the avgtime script or clone this repo
2. Make sure it is executable
3. (optional) Put it in your $PATH to be able to call it from anywhere

