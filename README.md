# dev_ShellCmds
Bash Shell Notes and Workspace

#### Time Related Commands
```
$MONTH="Sep-2021"
$find . -maxdepth 1 -type d -newermt "01-$MONTH -1 sec" -and -not -newermt "01-$MONTH +1 MONTH -1 sec" -exec mv {} sep21 \;

$find /. -mtime +30 -maxdepth 1 -type d
```
