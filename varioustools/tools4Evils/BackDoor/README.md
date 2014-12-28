BackDoor
===========

A simple BackDoor

Arch
		Backdoor
		   /\
	  Client Server	
	  		   /\
	  	  Loader Dll


Server
1. Extract Loader.exe and dll to Sys Dir (Store by PE's Resource)
2. Modify Reg to Autorun(via ActiveX) //HKEY_LOCALMACHINE\SOFTWARE\Microsofe\Active Setup\Installed Components  jst 4 once,once the info exsits It's would not autorun
3. self Delete

Loader
1. Raise the Privilege of Process
2. Create A IE Process.
3. inject the Dll (via CreateRemoteTHread)
4. Del Reg Keys about ActiveX(4 server could autorun everytime)

Dll (the Mainly Backdoor)
via Socket
RemoteCMD via IPC here Pipe
URLDownloadToFile


Client
interactive via Socket