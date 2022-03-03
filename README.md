# libxml2-2.9.10
Built version of libxml2-2.9.10

## Way to go
1. Build the `libxml2.so.2.9.10` file locally using the install script and then pass it to the container
2. Locate it at `/usr/local/lib`
3. Create a symlink `libxml2.so.2`, otherwise this version won't be detected

Result:
```
(venv) /usr/local/lib # ls -la
lrwxrwxrwx    1 root     root            17 Mar  3 14:03 libxml2.so.2 -> libxml2.so.2.9.10
-rwxr-xr-x    1 root     root       6197904 Mar  3 13:49 libxml2.so.2.9.10
```
