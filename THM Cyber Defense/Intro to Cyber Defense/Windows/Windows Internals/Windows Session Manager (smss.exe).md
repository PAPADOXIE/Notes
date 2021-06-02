## smss.exe

#### Includes
- win32k.sys (kernel mode)
- winsrv.dll (user mode)
- csrss.exe (user mode)

#### Starts

##### Session 0 (Isolated OS Session)
- csrss.exe (Windows Subsystem)
- wininit.exe
- 
##### Session 1 (User Session)
- winlogon.exe

#### Creates
- Environment Variables
- Virtual Memory Paging Files

#### Normal Behavior
- Image Path:  %SystemRoot%\\System32\\smss.exe
- Parent Process:  System
- Number of Instances:  One master instance and child instance per session. The child instance exits after creating the session.
- User Account:  Local System
- Start Time:  Within seconds of boot time for the master instance