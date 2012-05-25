---
layout: page
title: "Madrona Appliance"
active: developer
---
{% include JB/setup %}
<div class="row">
<div class="span6">
<h1>Madrona Appliance</h1>
<p>We've packaged up everything you need to try out Madrona into a downloadable virtual machine.  You can use it with VirtualBox or VMWare without having to set up a server or install any other software. 
</p>
<p>The Madrona virtual machine was built on Ubuntu 12.04 Server (32-bit) with an LXDE desktop. It comes with Madrona and all of it's dependencies installed so you can start building sites right out of the box. 
</p>
<ol>
	<li>Download and install <a href="http://www.virtualbox.org/">VirtualBox</a>.</li>
	<li>Download the <a href="https://s3.amazonaws.com/madrona_vm/madrona_virtual_v3.ova">Madrona Appliance</a> (~ 1.1GB)</li>
	<li>File > Import Applicance > select the .ova file.</li>
	<li>Set up networking. In the VM Manager,
		<ul>
			<li>select the Madrona VM</li>
			<li>click the "Settings" icon</li>
			<li>click on "Network"</li>
			<li>Check that your network card is listed in the "Name" field</li>
			<li>Click "OK"</li>
		</ul>
	</li>
	<li>Start and follow instructions on screen</li>
	<li>See the <a href="http://ecotrust.github.com/madrona/docs/tutorial_appgen.html">tutorial</a> for more detailed instructions.</li>
</ol>

<h2>Known Issues</h2>
<ul>
	<li>User must set up hosts file</li>
	<li>The network interface is hardcoded in the ova xml file and must be (re)set manually by virtualbox</li>
	<li>You can't create a Folder named "Folder"</li>
</ul>

</div>
<div class="span6">
<h2>Verify Integrity of the download</h2>
<table class="table table-condensed">
	<tr><th>MD5 Checksum</th><th>filesize</th><th>filename</th></tr>
	<tr><td>8e31e61c9859d9e1e9250227fd9b687e</td><td>1095751680</td><td>madrona_virtual_v1.ova</td></tr>
	<tr><td>4c0e63843548e7e7c5b02c3b4599be5e</td><td>1174923264</td><td>madrona_virtual_v2.ova</td></tr>
	<tr><td>8e56fc0b335e54d515036ea71c4fd22f</td><td>1187844096</td><td>madrona_virtual_v3.ova</td></tr>
</table>
</div>
</div>