# Disable the Firewall
esxcli network firewall set --enabled false
#Pick your Version of ESXi Hypervisor you want
#7.0.0
esxcli software profile update -p ESXi-7.0bs-16321839-standard -d
https://hostupdate.vmware.com/software/VUM/PRODUCTION/main/vmw-depot-index.xml
#7.0b
esxcli software profile update -p ESXi-7.0b-16324942-standard -d
https://hostupdate.vmware.com/software/VUM/PRODUCTION/main/vmw-depot-index.xml
#7.0U1
esxcli software profile update -p ESXi-7.0.1-16850804-standard -d
https://hostupdate.vmware.com/software/VUM/PRODUCTION/main/vmw-depot-index.xml
#7.0U1a
esxcli software profile update -p ESXi-7.0U1a-17119627-standard -d
https://hostupdate.vmware.com/software/VUM/PRODUCTION/main/vmw-depot-index.xml
#7.0U1b
esxcli software profile update -p ESXi-7.0U1b-17168206-standard -d
https://hostupdate.vmware.com/software/VUM/PRODUCTION/main/vmw-depot-index.xml
#7.0U1sc
esxcli software profile update -p ESXi-7.0U1sc-17325020-standard -d
https://hostupdate.vmware.com/software/VUM/PRODUCTION/main/vmw-depot-index.xml
#7.0U1c
esxcli software profile update -p ESXi-7.0U1c-17325551-standard -d
https://hostupdate.vmware.com/software/VUM/PRODUCTION/main/vmw-depot-index.xml
#7.0U1d
esxcli software profile update -p ESXi-7.0U1d-17551050-standard -d
https://hostupdate.vmware.com/software/VUM/PRODUCTION/main/vmw-depot-index.xml
#7.0U2a
esxcli software profile update -p ESXi-7.0U2a-17867351-standard -d
https://hostupdate.vmware.com/software/VUM/PRODUCTION/main/vmw-depot-index.xml
#enable firewall
esxcli network firewall set --enabled true
#reboot server
reboot
