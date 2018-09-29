# server
```
 sudo apt install linux-tools-`unamr -r`
 sudo modprobe usbip-host 
 # or echo "usbip-host" >>/etc/modules
 
 # start daemon
 /usr/lib/linux-tools/`uname -r`/usbipd &

 # bind local device to uhost
 /usr/lib/linux-tools/`uname -r`/usbip list -l 
 /usr/lib/linux-tools/`uname -r`/usbip list -b 1-1.3 

 
```
# client
```
 sudo apt install linux-tools-`unamr -r`
 sudo modprobe vhci-hcd
 # or echo "vhci-hcd" >>/etc/modules
 
 # start daemon

 # bind local device to uhost
 /usr/lib/linux-tools/`uname -r`/usbip list -r  $remote_host 
 /usr/lib/linux-tools/`uname -r`/usbip attach -r $remote_host -b 1-1.3 

 
```
https://github.com/solarkennedy/wiki.xkyle.com/wiki/USB-over-IP-On-Ubuntu

https://github.com/torvalds/linux/tree/master/tools/usb/usbip
