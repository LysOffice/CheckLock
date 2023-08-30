# CheckLock

Changer les éléments dans le script PS1

Installer en service : (en powershell) 

$PathPowerShell = (Get-Command Powershell).Source
./nssm.exe install LockCheck $PathPowerShell "C:\LCL-Info\LockCheck\LockCheck.ps1"

Lancer le service 


Pour relancer suite un arrêt : (admin)
net start lanmanserver
net start browser


