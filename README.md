# A Kernel Seedling
TODO: intro

## Building
```shell
make
```

## Running
```shell
sudo insmod proc_count.ko
cat /proc/count
```
TODO: results?
A single integer is printed. (When i ran it that number was 167).
## Cleaning Up
```shell
sudo rmmod proc_count
```

## Testing
```python
python -m unittest
```
TODO: results?
All tests passed should return OK. When I ran this it returned "Ran 3 tests in 3.781s OK"
Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

```shell
uname -r -s -v
```
Linux 5.14.8-arch1-1