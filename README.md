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