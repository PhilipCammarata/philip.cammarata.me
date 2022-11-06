# Lab

I'm a big fan of the [Windows Admin Center](https://www.microsoft.com/en-us/windows-server/windows-admin-center) (WAC).  Being web based means I can use any operating system and just add one more tab to my browser.

```powershell
Start-BitsTransfer -Source https://go.microsoft.com/fwlink/p/?linkid=2194936 -Destination WindowsAdminCenter.msi
msiexec /i WindowsAdminCenter.msi /qn /L*v log.txt SME_PORT=443 SSL_CERTIFICATE_OPTION=generate
```
