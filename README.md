# VMware-Download-Links

Login to the Broadcom Account. Registering a new account if neccessary.

Once logged in, navigate to:

https://support.broadcom.com/group/ecx/downloads 

or

https://support.broadcom.com/group/ecx/free-downloads

or click on the links below.

## VMware Player Download

https://support.broadcom.com/group/ecx/productdownloads?subfamily=VMware%20Workstation%20Player&freeDownloads=true



## Vmware Workstation Pro Download

https://support.broadcom.com/group/ecx/productdownloads?subfamily=VMware%20Workstation%20Pro&freeDownloads=true



## Vmware Tools Download

https://support.broadcom.com/group/ecx/productdownloads?subfamily=VMware%20Tools&freeDownloads=true



### Spectre / Meltdown Side Channel Mitigation VMX setting.

To switch off Side Channel mitigation add the following line to the closed VM .vmx file.

This will speed up the operation of a virtual machine considerably!

```
ulm.disableMitigations = "TRUE"
```

### MS Windows Defender - Exclusions

https://learn.microsoft.com/en-us/defender-endpoint/configure-process-opened-file-exclusions-microsoft-defender-antivirus

https://learn.microsoft.com/en-us/defender-endpoint/configure-process-opened-file-exclusions-microsoft-defender-antivirus

https://learn.microsoft.com/en-us/defender-endpoint/configure-extension-file-exclusions-microsoft-defender-antivirus

https://learn.microsoft.com/en-us/defender-endpoint/configure-server-exclusions-microsoft-defender-antivirus#hyper-v-exclusions

Common Mistakes

https://learn.microsoft.com/en-us/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus#folder-locations

https://learn.microsoft.com/en-us/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus#file-extensions

https://learn.microsoft.com/en-us/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus#processes


https://learn.microsoft.com/en-us/defender-endpoint/indicator-ip-domain

https://learn.microsoft.com/en-us/defender-endpoint/indicators-overview

```
You can use IP and URL/Domain indicators to manage site access.

To block connections to an IP address, type the IPv4 address in dotted-quad form (e.g. 8.8.8.8). For IPv6 addresses, specify all 8 segments (e.g. 2001:4860:4860:0:0:0:0:8888). Note that wildcards and ranges are not supported.

To block connections to a domain and any of its subdomains, specify the domain (e.g. example.com). This indicator will match example.com as well as sub.example.com and anything.sub.example.com.

To block a specific URL path, specify the URL path (e.g. https://example.com/block). This indicator will match resources under the /block path on example.com. Note that HTTPS URL paths will only be matched in Microsoft Edge; HTTP URL paths can be matched in any browser.
```


Windows Security -> Virus & Threat Protection -> Virus & Threat Protection Settings - Manage Settings -> Exclusions


OR Powershell
```
Get-MpPreference
Set-MpPreference
Add-MpPreference
Remove-MpPreference
```

```
ExclusionExtension
ExclusionIpAddress
ExclusionPath
ExclusionProcess
```


All Exe's Found
```
C:\Program Files (x86)\VMware\VMware Workstation\vmware.exe
C:\Program Files (x86)\VMware\VMware Workstation\7za.exe
C:\Program Files (x86)\VMware\VMware Workstation\autostart-helper.exe
C:\Program Files (x86)\VMware\VMware Workstation\containerd.exe
C:\Program Files (x86)\VMware\VMware Workstation\containerd-shim-crx-v2.exe
C:\Program Files (x86)\VMware\VMware Workstation\drvInst64.exe
C:\Program Files (x86)\VMware\VMware Workstation\mkisofs.exe
C:\Program Files (x86)\VMware\VMware Workstation\vmcli.exe
C:\Program Files (x86)\VMware\VMware Workstation\vmnat.exe
C:\Program Files (x86)\VMware\VMware Workstation\vmnetcfg.exe
C:\Program Files (x86)\VMware\VMware Workstation\VMnetDHCP.exe
C:\Program Files (x86)\VMware\VMware Workstation\vmplayer.exe
C:\Program Files (x86)\VMware\VMware Workstation\vmrest.exe
C:\Program Files (x86)\VMware\VMware Workstation\vmrun.exe
C:\Program Files (x86)\VMware\VMware Workstation\vmss2core.exe
C:\Program Files (x86)\VMware\VMware Workstation\vmUpdateLauncher.exe
C:\Program Files (x86)\VMware\VMware Workstation\vmware-authd.exe
C:\Program Files (x86)\VMware\VMware Workstation\vmware-autostart.exe
C:\Program Files (x86)\VMware\VMware Workstation\vmware-kvm.exe
C:\Program Files (x86)\VMware\VMware Workstation\vmware-remotemks.exe
C:\Program Files (x86)\VMware\VMware Workstation\vmware-tray.exe
C:\Program Files (x86)\VMware\VMware Workstation\vmware-vdiskmanager.exe
C:\Program Files (x86)\VMware\VMware Workstation\vnetlib.exe
C:\Program Files (x86)\VMware\VMware Workstation\vnetlib64.exe
C:\Program Files (x86)\VMware\VMware Workstation\vnetsniffer.exe
C:\Program Files (x86)\VMware\VMware Workstation\vnetstats.exe
C:\Program Files (x86)\VMware\VMware Workstation\zip.exe

C:\Program Files (x86)\VMware\VMware Workstation\x64\mksSandbox.exe
C:\Program Files (x86)\VMware\VMware Workstation\x64\mksSandbox-debug.exe
C:\Program Files (x86)\VMware\VMware Workstation\x64\mksSandbox-stats.exe
C:\Program Files (x86)\VMware\VMware Workstation\x64\tpm2emu.exe
C:\Program Files (x86)\VMware\VMware Workstation\x64\vmware-vmx.exe
C:\Program Files (x86)\VMware\VMware Workstation\x64\vmware-vmx-debug.exe
C:\Program Files (x86)\VMware\VMware Workstation\x64\vmware-vmx-stats.exe

C:\Program Files (x86)\Common Files\VMware\USB\vmware-usbarbitrator.exe
C:\Program Files (x86)\Common Files\VMware\USB\vmware-usbarbitrator64.exe
C:\Program Files (x86)\Common Files\VMware\USB\vnetlib.exe
C:\Program Files (x86)\Common Files\VMware\USB\vnetlib64.exe

C:\Program Files (x86)\Common Files\VMware\USB\DriverCache\vnetlib.exe
C:\Program Files (x86)\Common Files\VMware\USB\DriverCache\vnetlib64.exe

C:\Windows\SysWOW64\vmnetdhcp.exe
C:\Windows\SysWOW64\vmnat.exe
```



Folders
```
C:\Program Files (x86)\VMware
C:\Users\Admin1\Documents\Virtual Machines
C:\Program Files (x86)\Common Files\VMware
```
```
PS C:\WINDOWS\system32> Add-MpPreference -ExclusionPath "C:\Program Files (x86)\VMware"
PS C:\WINDOWS\system32> Add-MpPreference -ExclusionPath "C:\Users\Admin1\Documents\Virtual Machines"
PS C:\WINDOWS\system32> Add-MpPreference -ExclusionPath "C:\Program Files (x86)\Common Files\VMware"
```

```
PS C:\WINDOWS\system32> $ExclPath = Get-MpPreference
PS C:\WINDOWS\system32> $ExclPath.ExclusionPath
C:\Program Files (x86)\Common Files\VMware
C:\Program Files (x86)\VMware
C:\Users\Admin1\Documents\Virtual Machines
```


## Processes to Exclude
A Process can be excluded by its Image Name which is the filename without the path, or by the full path and image name.
eg
Image Name:```vmware.exe```
Full Path:```C:\Program Files (x86)\VMware\VMware Workstation\vmware.exe```

or by a wildcard
eg
```
C:\Program Files (x86)\VMware\VMware Workstation\*
```

```
PS C:\WINDOWS\system32> Add-MpPreference -ExclusionProcess "C:\Program Files (x86)\VMware\*"
PS C:\WINDOWS\system32> Add-MpPreference -ExclusionProcess "C:\Program Files (x86)\Common Files\VMware\*"
PS C:\WINDOWS\system32> Add-MpPreference -ExclusionProcess "C:\Windows\SysWOW64\vmnetdhcp.exe"
PS C:\WINDOWS\system32> Add-MpPreference -ExclusionProcess "C:\Windows\SysWOW64\vmnat.exe"
```

```
PS C:\WINDOWS\system32> $ExclProcess = Get-MpPreference
PS C:\WINDOWS\system32> $ExclProcess.ExclusionProcess
C:\Program Files (x86)\Common Files\VMware\*
C:\Program Files (x86)\VMware\*
C:\Windows\SysWOW64\vmnat.exe
C:\Windows\SysWOW64\vmnetdhcp.exe
```
