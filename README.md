# extract

extract debugs memory leak of a running process with ltrace.

# build

```
$ make extract
```

# usage

```
$ ltrace -p TARGET_PROCESS_PID -e malloc+free+calloc+realloc-@libc* -o target_file.txt
$ extrace target_file.txt
```


