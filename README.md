# CheckLock

Changer les éléments dans le script PS1 (Lecteur et chemin du fichier Log)

Pour le service, téléchargez NSSM
https://nssm.cc/download

Mettre le script et NSSM dans un dossier

Installer en service : (en powershell) 

$PathPowerShell = (Get-Command Powershell).Source
./nssm.exe install LockCheck $PathPowerShell "...{chemin}...\LockCheck.ps1"

Lancer le service 

Pour relancer suite un arrêt : (admin)
net start lanmanserver
net start browser


