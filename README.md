iniDiff

iniDiff is a php script created to compare two .ini/config files.

the File format given to iniDiff has to similar to:
```
[section]
option = value
```

Output will look as follows:
```
[root@dmilbert /home/dmilbert/ ] # iniDiff file1.ini file2.ini 
┌──────══ [mysqld]
├ << query_cache_size = 192M
├ << innodb_buffer_pool_size = 512M
├ << long_query_time = 5
├ >> max_connections = 100
├ >> wait_timeout = 3600
├ >> query_cache_type = 0 
├ >> innodb_file_per_table = on
├ >> innodb_buffer_pool_size = 4096M
└────────
```
