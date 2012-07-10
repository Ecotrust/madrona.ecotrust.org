---
layout: page
title: "Madrona Appliance"
active: developer
---
{% include JB/setup %}
<div class="row">
<div class="span8">
<h1>Madrona Appliance</h1>
<p>We've packaged everything you need to test-drive Madrona into a self-contained appliance (virtual machine) that can be run on your local system.  This appliance is untested in production use.  Experience with virtual computing and networking is helpful but not required.  Follow the instructions below to get up and running and you'll be ready for the step-by-step tutorial.
</p>

<p>Requirements: a Windows or OSX system that can run Google Earth</p>

<ol>
	<li><a href="http://www.virtualbox.org/">Download</a> and install VirtualBox</li>
		<ul>
			<li>Supports Windows, OSX and Linux</li>
			<li>Note: VMWare ESXi can also be used with some <a href="https://groups.google.com/forum/?fromgroups#!topic/madrona-users/R7qZvFCSCQg">additional work</a>.</li>
		</ul>
	<li><a href="https://s3.amazonaws.com/madrona_vm/madrona_virtual_v3.ova">Download</a> the Madrona Appliance</li>
		<ul>
			<li>~ 1.1GB in size</li>
			<li>Operating system: Ubuntu 12.04 Server 32-bit</li>
			<li>Desktop: LXDE</li>
		</ul>	
	<li>(Optionally) Verify the integrity of the download</li>
		<ul>
			<li>Filename: madrona_virtual_v3.ova</li>
			<li>Filesize: 1187844096 bytes</li>
			<li>Checksum: 8e56fc0b335e54d515036ea71c4fd22f</li>
		</ul>
	<li>Import the Madrona appliance into VirtualBox</li>
		<ul>
			<li>File > Import Applicance > select the .ova file.</li>
		</ul>
	<li>Set up VirtualBox networking</li>
		<ul>
			<li>Select the newly imported Madrona VM</li>
			<li>Click the "Settings" icon</li>
			<li>Click on "Network"</li>
			<li>Select your network adapter in the 'Name' field.  If you have multiple adapters such as for wired and wireless, select the one that you are currently using for your internet connection.</li>
			<li>Click "OK"</li>
		</ul>
	<li>Start the virtual machine</li>
		<ul>			
			<li>The virtual machine will load for a minute or two, be patient.</li>
			<li>If you get a network error, go back and verify the previous step was completed successfully.</li>
			<li>If everything was successful you will be presented with a 'Welcome to the Madrona Virtual Machine' screen.</li>
		</ul>	
	<li><a href="{{BASE_PATH}}/developer/tutorial/madrona_appliance.html">Begin</a> the Madrona appliance tutorial</li>
</ol>
</div>
</div>