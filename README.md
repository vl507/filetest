# AD Downloader

This program downloads data from Teoco Netrac AutoDiscovery csv files to SURMS Database.


## Requirements

AD Downloader requires the following software:

- Ubuntu/Debian/CentOS/RHEL
- Python 3.4.2 or higher
- python cx_Oracle module 5.1.3 (maybe others also works)


## Run program

```
./run_program.sh
```

## Run tests

```
./run_tests.sh
```

Tests check db connection, existence of cvs files and ip addresses which should be present in Import_NE_*.csv file

## Main config file

[conf/config.ini](conf/config.ini)

## Input IP list file

[conf/ip_list.conf](conf/ip_list.conf)

## Convertion algorithms

[docs](docs)
