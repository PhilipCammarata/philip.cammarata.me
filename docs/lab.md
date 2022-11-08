---
hide:
  - toc
---

# Lab

## Windows Admin Center

[Windows Admin Center](https://www.microsoft.com/en-us/windows-server/windows-admin-center) (WAC) is a great way to administrate a Windows server and is entirely web based so it can be used on a Mac or anything that has a modern browser.

``` { .powershell }
Start-BitsTransfer -Source https://go.microsoft.com/fwlink/p/?linkid=2194936 -Destination WindowsAdminCenter.msi
msiexec /i WindowsAdminCenter.msi /qn /L*v log.txt SME_PORT=443 SSL_CERTIFICATE_OPTION=generate
```

## Volume Setup

I have two disks, one 1TB HDD that came with the hardware and an 128GB SSD that I installed to contain the host operating system.

``` { .powershell }
Set-Volume -DriveLetter C -NewFileSystemLabel "OS"

Get-Disk -FriendlyName "Apple*" | `
    New-Partition -UseMaximumSize -DriveLetter D | `
    Format-Volume -FileSystem NTFS -NewFileSystemLabel "STORAGE"
```
