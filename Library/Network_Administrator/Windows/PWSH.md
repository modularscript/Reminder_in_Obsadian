
- Print profile location {settings} & path
	- PROFILE.CurrentUserCurrentHost
	- ExecutionPolicy { if not in developer mode better disable => (preventing scrips to execute) }
		- Get-ExecutionPolicy -List
		- Get-ExecutionPolicy -Scope Process
		- Get-ExecutionPolicy -Scope CurrentUser
		- Set-ExecutionPolicy -Scope LocalMachine
		- Set-ExecutionPolicy -Scope CurrentUser  
		- also Execution can be disabled in system settings etc.....
		 
- 
- 
- 