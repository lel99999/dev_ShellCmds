# dev_ShellCmds
Bash Shell Notes and Workspace

#### Time Related Commands
```
$MONTH="Sep-2021"
$find . -maxdepth 1 -type d -newermt "01-$MONTH -1 sec" -and -not -newermt "01-$MONTH +1 MONTH -1 sec" -exec mv {} sep21 \;
$find *.gz -mtime +120 -exec mv {} <directory> \;

$find /. -maxdepth 1 -type d -mtime +30

find . -maxdepth 1 -type d -mtime +1095 -ls > /tmp/artifacts_archive01.txt
 
```

##### Experimental
```
find . -maxdepth 1 -type d -mtime +1460 -exec `du -h | sort -n -r | head -n 10` {} \;
```

#### Moving Numerical Files/Directories
```
mv {1..100} <directory>
```

#### List Files/Directories by Size
```
du -a /<directory> | sort -n -r | head -n 10
```
