# Configuring a Full Backup for a Windows Server Protection Group

<PageHeader />

Navigate to "Inventory -> Protection Group -> Add to bacup -> Windows -> New job":

![Windows_Backup_9](./full_windows_backup_9.png)

Select the appropriate Job Mode:  

![Windows_Backup_10](./full_windows_backup_10.png)

Assign a meaningful name:  

![Windows_Backup_11](./full_windows_backup_11.png)

Select the Protection Group(s) or Individual Servers you wish to back-up:  

![Windows_Backup_12](./full_windows_backup_12.png)

Select the appropriate Backup Mode:  

![Windows_Backup_13](./full_windows_backup_13.png)

Select a storage location with adequate space to store these full backups:  

![Windows_Backup_14](./full_windows_backup_14.png)

Select any Guest Processing that needs to be done in order to facilitate restores:  

![Windows_Backup_15](./full_windows_backup_15.png)

Set a schedule for when the backups should be run:  

![Windows_Backup_16](./full_windows_backup_16.png)

Then "Apply" and "Finish":  

![Windows_Backup_17](./full_windows_backup_17.png)

Examples of simple Windows scripts to pause and resume jBASE:

pause.cmd

```
@echo off
set JBCRELEASEDIR=C:\jBASE5\CurrentVersion
set JBCGLOBALDIR=%JBCRELEASEDIR%
set PATH=%JBCRELEASEDIR\bin:%PATH%
%JBCRELEASEDIR%\bin\DB-PAUSE.exe >nul 2>&1
exit
```

resume.cmd

```
@echo off
set JBCRELEASEDIR=C:\jBASE5\CurrentVersion
set JBCGLOBALDIR=%JBCRELEASEDIR%
set PATH=%JBCRELEASEDIR\bin:%PATH%
%JBCRELEASEDIR%\bin\DB-RESUME.exe >nul 2>&1
exit
```

See [this page](./../../jspool-script&scheduled-task/README.md) for details on how to create a Windows scheduled task.  

Back to [Veeam](./../README.md)

  
<PageFooter />
