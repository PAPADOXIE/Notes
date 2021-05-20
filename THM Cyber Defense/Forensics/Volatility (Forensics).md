## Volatility

##### [[Volatility (Malware Analysis)#Guess profile to use]]

##### [[Volatility (Malware Analysis)#List Processes]]

##### [[Volatility (Malware Analysis)#List Process' DLL's]]

##### View Active Network Connections
	volatility -f <filename.raw> --profile=<profilename> netscan

##### View Hidden Processes
	volatility -f <filename.raw> --profile=<profilename> psxview
	
##### View Hidden Process Details
	volatility -f <filename.raw> --profile=<profilename> ldrmodules
	
##### Find Unexpected Patches in System DLL's
	volatility -f <filename.raw> --profile=<profilename> apihooks

Be careful of ``Hooking Module: <unknown>``

##### Dump Injected Code
	volatility -f <filename.raw> --profile=<profilename> malfind -D <Destination Directory>
	
##### Dump DLL List For a Process
	volatility -f <filename.raw> --profile=<profilename> --pid=<PID> dlldump -D <Destination Directory>
	
#### Also see [[Volatility (Malware Analysis)]]