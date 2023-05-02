# debug-tools

A place to put some useful scripts to use when debugging on Linux.

> Tested in Ubuntu 20.04

## ptrace_scope

Permanently sets ptrace_scope.

### ptrace_scope examples

**Setting ptrace_scope to 0:**

``` bash
./ptrace_scope 0
```

**Setting ptrace_scope to 1:**

``` bash
./ptrace_scope 1
```

## core-dump

Disables enables the creation of crash dumps with the format [workdir]/core.[PROCESS NAME].[PID].[SIGNAL].[TIME SINCE EPOCH]

### core-dump examples

**Enabling**

``` bash
./core-dump 
```

**Resetting the configuration (according to Ubuntu 20.04)**

``` bash
./core-dump --reset
```

## mem.sh

Displays the memory used by a process

``` bash
./mem.sh [PROCESS NAME]
```
