---
Name: Sqlps.exe
Description: Tool included with Microsoft SQL Server that loads SQL Server cmdlets.
Author: 'Oddvar Moe'
Created: '2018-05-25'
Commands:
  - Command: Sqlps.exe -noprofile
    Description: Drop into a SQL Server PowerShell console without Module and ScriptBlock Logging.
    Usecase: Execute PowerShell commands without ScriptBlock logging.
    Category: Execute
    Privileges: User
    MitreID: T1218
    MitreLink: https://attack.mitre.org/wiki/Technique/T1218
    OperatingSystem: Windows
Full_Path:
  - Path: C:\Program files (x86)\Microsoft SQL Server\100\Tools\Binn\sqlps.exe
Code_Sample:
  - Code:
Detection:
  - IOC:
Resources:
  - Link: https://twitter.com/bryon_/status/975835709587075072
Acknowledgement:
  - Person: Bryon
    Handle: '@bryon_'
---
