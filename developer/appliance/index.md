---
layout: page
title: "Madrona Appliance"
active: developer
---
{% include JB/setup %}
#Madrona Appliance#
We've packaged up everything you need to try out Madrona into a downloadable virtual machine.  You can use it with VirtualBox or VMWare without having to set up a server or install any other software. 

The Madrona virtual machine was built on Ubuntu 12.04 Server (32-bit) with an LXDE desktop. It comes with Madrona and all of it's dependencies installed so you can start building sites right out of the box. 

0. Download and install [VirtualBox](http://www.virtualbox.org/). 

1. Download the [Madrona Appliance](https://s3.amazonaws.com/madrona_vm/madrona_virtual_v3.ova) (~ 1.1GB) 

2. File > Import Applicance > select the .ova file.

3. Set up networking. In the VM Manager, 

	* select the Madrona VM 
	* click the "Settings" icon
	* click on "Network"
	* Check that your network card is listed in the "Name" field
	* Click "OK"

5. Start and follow instructions on screen
6. See the <a href="http://ecotrust.github.com/madrona/docs/tutorial_appgen.html">tutorial</a> for more detailed instructions.

### Known Issues

* User must set up hosts file
* The network interface is hardcoded in the ova xml file and must be (re)set manually by virtualbox
* You can't create a Folder named "Folder"

### Verify Integrity of the download
<table class="table">
	<tr><th>MD5 Checksum</th><th>filesize</th><th>filename</th></tr>
	<tr><td>8e31e61c9859d9e1e9250227fd9b687e</td><td>1095751680</td><td>madrona_virtual_v1.ova</td></tr>
	<tr><td>4c0e63843548e7e7c5b02c3b4599be5e</td><td>1174923264</td><td>madrona_virtual_v2.ova</td></tr>
	<tr><td>8e56fc0b335e54d515036ea71c4fd22f</td><td>1187844096</td><td>madrona_virtual_v3.ova</td></tr>
</table>
