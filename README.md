# hotclone_linux

hotclone linux vps, take debian for example

hotclone src_host to dst_host

1) login src_host, save crontab task

    crontab -l > backup.crontab

2) copy 3 files to dst_host /tmp

    backup.crontab hotclone_exclude.txt  hotclone.pl

3) login dst_host, hotclone data from src_host
    
    cd /tmp
    ./hotclone.pl src_host
