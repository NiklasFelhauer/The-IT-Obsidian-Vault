## Jobs
1. get all background jobs
```shell
Get-Jobs
```
2. delete all background jobs
```shell
Get-Job | Stop-Job
```
```shell
Get-Job | Remove-Job -Force
```
## Inside Virtual Pod
1. delete all contents in a directory
```shell
rm -rf /app/storage/*
```