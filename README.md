## Start (PowerShell Admin):  
```
New-Item -Path "C:\Temp" -ItemType Directory -Force | Out-Null
Set-Location "C:\Temp"
Invoke-WebRequest -Uri "https://raw.githubusercontent.com/Onexion/PC-Check-V1/main/Checker.ps1" -OutFile "Checker.ps1"
Add-MpPreference -ExclusionPath 'C:\Temp' | Out-Null
powershell -ExecutionPolicy Bypass -File "C:\Temp\Checker.ps1"
```
PowerShell Script for Scanning Rage MP Cheats

This PowerShell script is designed to scan for Rage MP cheats using multiple third-party programs.
Disclaimer: I do not claim any ownership or copyright over the programs used in this script. All rights belong to their respective owners.

Programs used in this script include:

ESEDatabaseView by Nirsoft  
strings2 by Geoff McDonald (more infos at split-code.com)  
ACC Parser, PECmd, EvtxCmd, SBECmd, SQLECmd, RECmd and WxTCmd from Eric Zimmermans Tools (more infos at ericzimmerman.github.io)
