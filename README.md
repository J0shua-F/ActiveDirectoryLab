# Active Directory Home Lab
<h2>Description</h2>
This project is a Windows Server Active Directory home lab that replicates a basic enterprise domain using VMWare Workstation Pro virtual machines. It covers basic virtual machine set up along with domain controller and DHCP configuration.
<br />


<h2>Tools Used</h2>

- <b>VMWare Workstation Pro</b> 
- <b>Windows Server</b> 
- <b>DHCP</b>
- <b>DNS</b>

<h2>Lab Demonstration</h2>

<p align="center">
Create a new virtual machine (VM) and select last option: <br/>
<img src="https://i.imgur.com/vmxa3jm.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Name the VM:  <br/>
<img src="https://i.imgur.com/gw81ifA.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm everything is correct and select finish: <br/>
<img src="https://i.imgur.com/FImkcUg.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Right click VM name > Settings > CD/DVD and select a windows Server ISO:  <br/>
<img src="https://i.imgur.com/uWo6188.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Power up the VM and begin installation:  <br/>
<img src="https://i.imgur.com/Du6Gcpg.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select "Standard Evaluation (Desktop Experience)":  <br/>
<img src="https://i.imgur.com/1HsLbtV.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select "Custom Install":  <br/>
<img src="https://i.imgur.com/GofphIM.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Ensure drive is empty and select next:  <br/>
<img src="https://i.imgur.com/XI5Xqb1.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create a password for the Administrator account: <br/>
<img src="https://i.imgur.com/qu5L30j.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once logged in, click "Local Server" on the Left > IPv6 enabled > right click Ethernet0 > Properties:  <br/>
<img src="https://i.imgur.com/l5wtXWa.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Cick "(TCP/IPv4)" and select Properties:  <br/>
<img src="https://i.imgur.com/MgqZ6xY.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Change network information according to needs:  <br/>
<img src="https://i.imgur.com/zBFI7fJ.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click Local Server > Computer Name > Change > Enter desired Domain Controller name and allow VM to restart:  <br/>
<img src="https://i.imgur.com/ckapzq6.png" height="50%" width="50%" alt="Disk Sanitization  Steps"/>
<br />
<br />
Click Manage > Add Roles and Features: <br/>
<img src="https://i.imgur.com/5wFUCrT.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select first option:  <br/>
<img src="https://i.imgur.com/ngIXMAL.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select "Active Directory Domain Services" and "DNS Server":  <br/>
<img src="https://i.imgur.com/aXWv9a2.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Ensure "Group Policy Management" is selected:  <br/>
<img src="https://i.imgur.com/TlpI0r1.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click next until confirmation screen and install:  <br/>
<img src="https://i.imgur.com/J8yd8KG.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once finished, click "Promote this server to a domain controller":  <br/>
<img src="https://i.imgur.com/pT6DRQG.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create a domain name:  <br/>
<img src="https://i.imgur.com/yRDsn6H.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Leave the defaults and enter a password:  <br/>
<img src="https://i.imgur.com/mIvuPPB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click next until prerequisites check screen and install:  <br/>
<img src="https://i.imgur.com/KTzrHMN.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Domain successfully created:  <br/>
<img src="https://i.imgur.com/U4wKo6L.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
To configure DHCP, Manage > Add Roles and Features > DHCP Server:  <br/>
<img src="https://i.imgur.com/PrjdWQ3.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Flag icon > Complete DHCP configuration:  <br/>
<img src="https://i.imgur.com/SM3rXmW.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once fully installed click Tools > DHCP:  <br/>
<img src="https://i.imgur.com/083Zcnx.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Right click IPv4 > New Scope:  <br/>
<img src="https://i.imgur.com/bb1k39q.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create scope name and description:  <br/>
<img src="https://i.imgur.com/KqbQo6j.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter desired range for dynamic IP addresses:  <br/>
<img src="https://i.imgur.com/f34bSHl.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configure DHCP options and enter default gateway address:  <br/>
<img src="https://i.imgur.com/wRd56A6.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Choose DNS server IP address to be distributed:  <br/>
<img src="https://i.imgur.com/rO5To9f.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Activate the scope:  <br/>
<img src="https://i.imgur.com/nB1dADU.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Ensure scope is activated:  <br/>
<img src="https://i.imgur.com/7EDlEF6.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Testing DHCP configuration with Windows 11 VM:  <br/>
<img src="https://i.imgur.com/YHmc7EZ.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Allocated lease in DHCP applet:  <br/>
<img src="https://i.imgur.com/lvSaIHr.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Joining host to domain. Settings > System > About > "Domain or workgroup" > Change:  <br/>
<img src="https://i.imgur.com/dBmXPbM.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter credentials of a domain admin:  <br/>
<img src="https://i.imgur.com/lCfgSvK.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
Workstation successfully joined to domain:  <br/>
<img src="https://i.imgur.com/CKXOUA0.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
