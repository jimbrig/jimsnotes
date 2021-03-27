# SFC Scannow and DISM Commands

 On windows these commands are crucial for keeping a clean system:

 1. The *System File Checker* - `sfc /scannow`
 2. The *Deployment Image Servicing and Management* tool - `DISM.exe`

*NOTE: these must be ran as an ADMINISTRATOR*

```powershell
# powershell or CMD as ADMIN

# system file checker
sfc /scannow

# DISM
Dism /Online /Cleanup-Image /ScanHealth
Dism /Online /Cleanup-Image /CheckHealth
Dism /Online /Cleanup-Image /RestoreHealth
```

On Windows 10, when you start noticing random errors, problems booting up, or features not working as expected, there's a good chance that one or multiple system files might have gone missing or corrupted for unknown reasons. Usually, problems with system files could occur as a result of an issue installing a system update, driver, or application, or while making changes to the installation manually.

## SFC

- Visit Microsoft's Docs on SFC - [Link](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/sfc)

If you happen to come across this issue, you can use the Windows 10 System File Checker (SFC), which is a command-line tool designed to scan the integrity and restore missing or corrupted system files with working replacements.

Use the System File Checker tool to repair damaged system files automatically or manually if the tool refuses to work.


## DISM

- Visit Microsoft's Official Docs on DISM - [Link](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/what-is-dism)

Deployment Image Servicing and Management (DISM.exe) is a command-line tool that can be used to service and prepare Windows images, including those used for Windows PE, Windows Recovery Environment (Windows RE) and Windows Setup. DISM can be used to service a Windows image (.wim) or a virtual hard disk (.vhd or.vhdx).

