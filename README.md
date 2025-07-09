### MS17-012 - COM Session Moniker EoP Exploit running within MSBuild.exe

Slightly modified version of James Forshaw's COM Session Moniker Exploit (MS17-012), which can be run within MSBuild.exe and can be used to Bypass Application Whitelisting solutions. 
This version of the exploit enumerates Active User sessions on a system (RDP/Citrix) and lets you choose in which user session you want to execute a custom Payload.
License: BSD 3-Clause

Save This File And Execute The Following Command:

```
C:\Windows\Microsoft.NET\Framework\v4.0.30319\msbuild.exe C:\Scripts\MS17-012.csproj

Or

C:\Windows\Microsoft.NET\Framework64\v4.0.30319\msbuild.exe C:\Scripts\MS17-012.csproj
```

Author and founder of the MSBuild Application Whitelisting Bypass code: Casey Smith, Twitter: @subTee
More Info: http://subt0x10.blogspot.nl/2016/09/bypassing-application-whitelisting.html

Author and founder of the COM Session Moniker EoP Exploit: James Forshaw, Twitter: @tiraniddo
More Info: https://bugs.chromium.org/p/project-zero/issues/detail?id=1021

### Advice for BlueTeams

* First make sure you apply the MS17-012 security patches.
* Use Applocker or Device Guard to block these kind of Attacks and make sure you monitor/block trusted binaries like msbuild.exe 
