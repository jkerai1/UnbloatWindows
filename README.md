# DecrapifyWindows
powershell script to undo the telemetry nonsense inside windows.

Please read the script inside of powershell editor before running as it may disable things you may use.

Script requires admin rights


Additionally consider:

net user Guest /active no  

Disable Guest account


Check for processes

Get-CimInstance -Class Win32_Process | Select-Object -Property Name, HandleCount, ProcessId, ParentProcessId, Path, CommandLine, WriteTransferCount, ReadTransferCount, WorkingSetSize
