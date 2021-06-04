## csrss.exe

- Makes the Windows API available to other processes
- Maps drive letters
- Handles the Windows shutdown process

#### Loads
- csrsrv.dll
- basesrv.dll
- winsrv.dll

#### Normal Behavior
- Image Path:  %SystemRoot%\\System32\\csrss.exe
- Parent Process:  smss.exe (Terminates after starting csrss.exe)
- Number of Instances:  Two or more
- User Account:  Local System
- Start Time:  Within seconds of boot time for the first 2 instances (for Session 0 and 1).  Start times for additional instances occur as new sessions are created, although often only Sessions 0 and 1 are created.