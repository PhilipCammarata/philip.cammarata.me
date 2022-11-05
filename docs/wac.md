# Windows Admin Center

I'm a big fan of the [Windows Admin Center](https://www.microsoft.com/en-us/windows-server/windows-admin-center) (WAC).  Being web based means I use any operating system and just add one more tab to my ever growing list.

I often reinstall my lab's operating systems based on what I'm learning so when I go for Windows Server I run these commands to download and install WAC.

```
Start-BitsTransfer https://download.microsoft.com/download/1/0/5/1059800B-F375-451C-B37E-758FFC7C8C8B/WindowsAdminCenter2110.2.msi
PS C:\Users\pcammarata\Downloads> msiexec /i WindowsAdminCenter2110.2.msi /qn /L*v log.txt SME_PORT=443 SSL_CERTIFICATE_OPTION=generate
```
