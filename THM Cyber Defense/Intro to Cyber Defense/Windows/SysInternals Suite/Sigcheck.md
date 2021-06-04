## Sigcheck
Shows file version number, timestamp info and digital signature details

#### Check for unsigned files in a folder
	sigcheck -u -e <Path to Folder>
	
#### Check for information about a program on VirusTotal
	sigcheck -u <Path to File|Folder>
	
#### Scan executable images regardless of extension
	sigcheck -e <Path to File|Folder>
	