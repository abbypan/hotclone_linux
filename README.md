# hotclone_linux

hotclone linux vps, take debian for example

hotclone src.xxx.com to dst.yyy.com

1) login src.xxx.com, save crontab task

    crontab -l > backup.crontab

2) copy 3 files to dst.yyy.com /tmp

    hotclone.pl
    hotclone_exclude.txt
    backup.crontab

3) login dst.yyy.com, hotclone data from src.xxx.com
    
    cd /tmp
    ./hotclone.pl src.xxx.com
