---
layout: page
title: "Madrona Appliance"
active: developer
---
{% include JB/setup %}
<div class="row">
<div class="span8">
<h1>Madrona Appliance</h1>
<p>We have packaged up everything you need to try out Madrona into a self-contained virtual machine that can be run on your local system without having to configure a server or install additional software. 
</p>
<ol>
	<li>Download and install <a href="http://www.virtualbox.org/">VirtualBox</a></li>
		<ul>
			<li>Note: VMWare can also be used</li>
		</ul>
	<li>Download the <a href="https://s3.amazonaws.com/madrona_vm/madrona_virtual_v3.ova">Madrona Appliance</a></li>
		<ul>
			<li>~ 1.1GB in size</li>
			<li>Operating system: Ubuntu 12.04 Server 32-bit</li>
			<li>Desktop: LXDE</li>
		</ul>	
	<li>Verify the integrity of the download</li>
		<ul>
			<li>Filename: madrona_virtual_v3.ova</li>
			<li>Filesize: 1187844096 bytes</li>
			<li>MD5 checksum: 8e56fc0b335e54d515036ea71c4fd22f</li>
		</ul>
	<li>Import the Madrona appliance into VirtualBox
		<ul>
			<li>File > Import Applicance > select the .ova file.</li>
		</ul>
	</li>
	<li>Set up VirtualBox networking
		<ul>
			<li>Select the newly imported Madrona VM</li>
			<li>Click the "Settings" icon</li>
			<li>Click on "Network"</li>
			<li>Select your network adapter in the 'Name' field.  If you have multiple adapters such as for wired and wireless, select the one that you are currently using for your internet connection.</li>
			<li>Click "OK"</li>
		</ul>
	</li>
	<li>Start the virtual machine</li>
		<ul>
			<li>If you get a network adapter error, go back and verify the previous step was completed</li>
			<li>The virtual machine will load for a minute or two, be patient.</li>
			<li>If everything is successful you will be presented with a 'Welcome to the Madrona Virtual Machine' screen.</li>
		</ul>	
	<li>You are now ready to begin the Madrona Appliance <a href="http://ecotrust.github.com/madrona/docs/tutorial_appgen.html">tutorial</a></li>
</ol>
</div>
</div>