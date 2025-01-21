# How to compile

```
make
```
Then choose a heap management scheme:

First fit
```
$ env LD_PRELOAD=lib/libmalloc-ff.so tests/ffnf
```
Next fit
```
$ env LD_PRELOAD=lib/libmalloc-nf.so tests/ffnf
```
Best fit
```
$ env LD_PRELOAD=lib/libmalloc-bf.so tests/bfwf
```
Worst fit
```
$ env LD_PRELOAD=lib/libmalloc-bf.so tests/bfwf
```
test1 and test2 run malloc and free calls
test3 checks for coalescing blocks
test4 checks for splitting and reusing blocks
```
make clean
```