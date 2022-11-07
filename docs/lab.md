---
hide:
  - toc
---

# Lab

## Windows Admin Center

[Windows Admin Center](https://www.microsoft.com/en-us/windows-server/windows-admin-center) (WAC).

``` { .powershell }
Start-BitsTransfer -Source https://go.microsoft.com/fwlink/p/?linkid=2194936 -Destination WindowsAdminCenter.msi
msiexec /i WindowsAdminCenter.msi /qn /L*v log.txt SME_PORT=443 SSL_CERTIFICATE_OPTION=generate
```

# Volume Setup

``` { .powershell }
Set-Volume -DriveLetter C -NewFileSystemLabel "OS"

Get-Disk -FriendlyName "Apple*" | `
    New-Partition -UseMaximumSize -DriveLetter D | `
    Format-Volume -FileSystem NTFS -NewFileSystemLabel "STORAGE"
```
