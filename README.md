# A Kernel Seedling
This lab is for CS111 at UCLA. The task was to design a kernel module that outputted every process currently running.

## Building
```shell
make
```

## Running
```shell
sudo insmod proc_count.ko
cat /proc/count
```
A single integer is printed.

## Cleaning Up
```shell
sudo rmmod proc_count
```

## Testing
```python
python -m unittest
```
All tests passed, should return OK

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

```shell
uname -r -s -v
```
Linux 5.14.8-arch1-1