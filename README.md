# Active Directory Lab Using PowerShell


<h2>Background</h2> 
<h4>This repository serves as a guide and resource for setting up a comprehensive Active Directory Home Lab using Oracle VM, Windows 10, and Windows Server 2019. This project demonstrates the creation of a functional environment with a Domain Controller, Active Directory, NAT, routing, DHCP, and automated user creation using PowerShell scripts.</h4>

<image src="https://i.imgur.com/SUGKNNb.jpg">

<h2>Prerequisites</h2>

<h4>1 Oracle VM VirtualBox </br>
2 Windows 10 and Windows Server 2019 ISOs </br>
3 Adequate hardware resources (RAM, CPU) for running multiple VMs</h4>

<h2>Installation Steps</h2>

<h4>

[1] Create Virtual Machines: 
  * Set up two VMs using Oracle VM: one for the Domain Controller and another for the client machine.<br>
</br><image src="https://i.imgur.com/4HpfSIQ.png"> <br>
</br>
  * Install Windows Server 2019 on Domain Controller VM<br>
  </br><image src="https://i.imgur.com/DQ6imMZ.jpg"> <br>
 </br> 
  * Assign two network adapters to the Domain Controller VM (one for internet access and the other for the private network).<br>
</br><image src="https://i.imgur.com/N63TH54.png"> <br>
</br>

[2] Configure IP addressing for the internal network. <br>
</br><image src="https://i.imgur.com/dDWuZV5.png"><br>
</br>


[3] Install Active Directory on the Domain Controller VM.<br>
</br><image src="https://i.imgur.com/bflJ9Q1.png"><br>
</br>
  * Create a domain and configure necessary settings.<br>
  </br>
</br><image src="https://i.imgur.com/GdWQRM3.png"><br>
</br>
</br><image src="https://i.imgur.com/uJiYrOM.png"><br>
</br>
</br><image src="https://i.imgur.com/DsqDZbB.png"><br>
</br>
</br><image src="https://i.imgur.com/Es3DRQi.jpg"><br>
</br>



[4] Configure NAT and routing on the Domain Controller to allow clients on the private network to access the internet.<br>
</br>
</br><image src="https://i.imgur.com/U39wIUJ.png"><br>
</br>
</br><image src="https://i.imgur.com/aUWGzpF.png"><br>
</br>
</br><image src="https://i.imgur.com/filLGv2.png"><br>
</br>
</br><image src="https://i.imgur.com/TJbZ5o2.png"><br>
</br>



[5] Set up DHCP on the Domain Controller to automatically assign IP addresses to client machines.<br>
</br>
</br><image src="https://i.imgur.com/5dcYqT6.png"><br>
</br>
</br><image src="https://i.imgur.com/GlbVnph.png"><br>
</br>
</br><image src="https://i.imgur.com/TEkQ2Q9.png"><br>
</br>
</br><image src="https://i.imgur.com/Ouj0OHU.png"><br>
</br>
</br><image src="https://i.imgur.com/DnyNDET.png"><br>
</br>
</br><image src="https://i.imgur.com/OAN6j1y.png"><br>
</br>
</br><image src="https://i.imgur.com/rIX7xsz.png"><br>
</br>

[6] Run a PowerShell script on the Domain Controller to automatically create a specified number of users in Active Directory.<br>
</br>
</br><image src="https://i.imgur.com/mxXwfkl.png"><br>
</br>
</br><image src="https://i.imgur.com/ge89llc.png"><br>
</br>
</br><image src="https://i.imgur.com/vWd5Yfj.png"><br>
</br>
</br><image src="https://i.imgur.com/burIZ9S.png"><br>
</br>





[7] Install Windows 10 on the client VM connected to the private VirtualBox network. Join the client machine to the domain and log in with one of the domain accounts created earlier.</h4><br>
</br><image src="https://i.imgur.com/8vb3YRB.jpg"><br>
</br>
</br><image src="https://i.imgur.com/Rp7PI8I.png"><br>
</br>
</br><image src="https://i.imgur.com/dLwu2tr.png"><br>
</br>
</br><image src="https://i.imgur.com/zPMdSA5.png"><br>
</br>
</br><image src="https://i.imgur.com/lUBdcd1.png"><br>
</br>
</br><image src="https://i.imgur.com/4zPv5Kl.png"><br>
</br>

