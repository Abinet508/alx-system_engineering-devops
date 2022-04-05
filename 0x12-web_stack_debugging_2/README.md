# 0x12. Web stack debugging #2

## Overview
This project was another webstack debugging project using pre-configured containers to fix issues with the various infrastructural tools

## Requirements
### Shell Scripts
* Allowed editors: `vi`, `vim`, `emacs`
* All your scripts will be tested on Ubuntu 14.04 LTS
* All your scripts should be exactly two lines long (`wc -l` file should print 2)
* All your files should end with a new line
* The first line of all your files should be exactly `#!/bin/bash`
* All your files must be executable

## Tasks
### Mandatory
**[0-iamsomeonelese](0-iamsomeonelese)** - takes one argument and runs the `whoami` command as the user passed in the argument
```
 # whoami
root

 # ./0-iamsomeonelese nginx
nginx

~# whoami
root
```

**[1-run_nginx_as_nginx](1-run_nginx_as_nginx)** - `nginx` must be running as the `nginx` user and must be listening to all active IPs on port `8080`
```
~# ps auxff | grep ngin[x]
nginx      884  0.0  0.0  77360  2744 ?        Ss   19:16   0:00 nginx: master process /usr/sbin/nginx
nginx      885  0.0  0.0  77712  2772 ?        S    19:16   0:00  \_ nginx: worker process
nginx      886  0.0  0.0  77712  3180 ?        S    19:16   0:00  \_ nginx: worker process
nginx      887  0.0  0.0  77712  3180 ?        S    19:16   0:00  \_ nginx: worker process
nginx      888  0.0  0.0  77712  3208 ?        S    19:16   0:00  \_ nginx: worker process
```
### Advanced

**[100-fix_in_7_lines_or_less](100-fix_in_7_lines_or_less)** - Using what you did for `task #1`, make your fix `short` and `sweet`.

