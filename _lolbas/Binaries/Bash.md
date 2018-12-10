---
Name: Bash.exe
Description: File used by Windows subsystem for Linux
Author: 'Oddvar Moe'
Created: '2018-05-25'
Commands:
  - Command: bash.exe -c calc.exe
    Description: Executes calc.exe from bash.exe
    Usecase: Performs execution of specified file, can be used as a defensive evasion.
    Category: Execute
    Privileges: User
    MitreID: T1218
    MitreLink: https://attack.mitre.org/wiki/Technique/T1218
    OperatingSystem: Windows 10
  - Command: bash.exe -c calc.exe
    Description: Executes calc.exe from bash.exe
    Usecase: Performs execution of specified file, can be used to bypass Application Whitelisting.
    Category: AWL Bypass
    Privileges: User
    MitreID: T1218
    MitreLink: https://attack.mitre.org/wiki/Technique/T1218
    OperatingSystem: Windows 10
Full_Path:
  - Path: C:\Windows\System32\bash.exe
  - Path: C:\Windows\SysWOW64\bash.exe
Code_Sample: 
  - Code:
Detection:
  - IOC: Child process from bash.exe
Resources:
  - Link: https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-control/microsoft-recommended-block-rules
Acknowledgement:
  - Person: Alex Ionescu
    Handle: '@aionescu'
---