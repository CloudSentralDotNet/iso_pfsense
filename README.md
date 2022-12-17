Download our selected pfsense isos' at  https://github.com/CloudSentralDotNet/iso_pfsense/releases     

or alternatively use these direct download links:       

* https://github.com/CloudSentralDotNet/iso_pfsense/releases/download/2.6.0/pfSense-CE-2.6.0-RELEASE-amd64.img
* https://github.com/CloudSentralDotNet/iso_pfsense/releases/download/2.5.2/pfSense-CE-2.5.2-RELEASE-amd64.iso
* https://github.com/CloudSentralDotNet/iso_pfsense/releases/download/2.4.4/pfSense-CE-2.4.4-RELEASE-amd64.img     
* https://github.com/CloudSentralDotNet/iso_pfsense/releases/download/2.4.2/pfSense-CE-2.4.2-RELEASE-amd64.img  
* https://github.com/CloudSentralDotNet/iso_pfsense/releases/download/2.3.5/pfSense-CE-2.3.5-RELEASE-amd64.img    


Burning ISO / IMG to a USB Drive using 'dd'

* Insert USB drive but do not mount it.
* Check drive designation by running 'sudo lsblk' in a console.
* Run 'sudo dd bs=4M if=/path/to/pfsense.iso  of=/dev/sdX   status=progress  &&  sync' 
  Replace sdX with your USB drive designation, for example: sdc (be very careful here!).
* The sync part is important, do not omit it!

After dd command finishes, your drive is ready.
