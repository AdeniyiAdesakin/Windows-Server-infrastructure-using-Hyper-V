![image](https://github.com/user-attachments/assets/efc33d99-e7af-47c1-971f-ef100af1edd8)<h1>Windows Server Infrastructure using Hyper-V</h1>
<p>In this project, I set up windows server infrastructure using Hyper V - a Microsoft's hardware virtualization product. This infrastructure includes an Active Directory User and Computer server, a Member server and a Client computer</p>
<h3>*Enabling Hyper-V for use on Windows 10 </h3>
<p>1. To enable Hyper V for use on my Windows 11 Pro, I did the following; From the start charm, searched for Control Panel, then clicked on Programs </p>
<p align="center"><img src="https://i.imgur.com/MsLlk8T.png" height="50%" width="50%" alt="image"/>

<p>2. On the Control Panel>Programs page, clicked on Turn Windows features on or off </p>
<p align="center"><img src="https://i.imgur.com/Q3PEBRk.png" height="50%" width="50%" alt="image"/>

<p>3. From the Turn windows features on or off page, selected Hyper V, then clicked OK</p>
<p align="center"><img src="https://i.imgur.com/aAcbc3V.png" height="50%" width="50%" alt="image"/>

<p>4. After the request changes have been completed, you are asked to restart your computer.</p>
<p align="center"><img src="https://i.imgur.com/fEPs1tY.png" height="50%" width="50%" alt="image"/>

<br>
<br>

<h3>*Installing and preparing Windows Servers and Windows 10 in Hyper-V.</h3>
<p><b>Windows Server with Active Directory Domain Services (ADDS)</b></p>
<p>1. To install Windows Server 2019(ADDS) on Hyper V; from the Hyper V manager, right click on the Computer name, go to New, then Virtual Machine</p>
<p align="center"><img src="https://i.imgur.com/QGOINFy.png" height="50%" width="50%" alt="image"/>

<p>2. On the Before you begin page, click NEXT</p>
<p align="center"><img src="https://i.imgur.com/1X44jd3.png" height="50%" width="50%" alt="image"/>

<p>3. On the Specify Name and Location page, type in a descriptive name(ADDS), then click NEXT</p>
<p align="center"><img src="https://i.imgur.com/CYgWw1e.png" height="50%" width="50%" alt="image"/>

<p>4. On the Specify Generation select Generation 2(more features) and click NEXT</p>
<p align="center"><img src="https://i.imgur.com/jjYjvtu.png" height="50%" width="50%" alt="image"/>

<p>5. On the Assign memory, leave it at default and uncheck the Use Dynamic Memory for this Virtual Ma-chine(this prevent guest virtual machine memory flexibility)</p>
<p align="center"><img src="https://i.imgur.com/QTKtNmk.png" height="50%" width="50%" alt="image"/>

<p>6. On the Configure Networking, switch to Default Switch and click NEXT</p>
<p align="center"><img src="https://i.imgur.com/nVzXB1j.png" height="50%" width="50%" alt="image"/>

<p>7. On the Connect Virtual Hard Disk page, input 30 GB instead of 127 GB, then click NEXT</p>
<p align="center"><img src="https://i.imgur.com/ta9EHCO.png" height="50%" width="50%" alt="image"/>

<p>8. On the Installation Options page, select Install an Operating system from a bootable image file, then browse and select the ISO image file where it is located on your computer, then click NEXT</p>
<p align="center"><img src="https://i.imgur.com/VqR9RjM.png" height="50%" width="50%" alt="image"/>

<p>9. On the Completing the new virtual machine wizard page, click FINISH</p>
<p align="center"><img src="https://i.imgur.com/beEcTFU.png" height="50%" width="50%" alt="image"/>

<BR>

<h3>Configuration</h3>
<p>1. While on the Hyper V Manager, right click on the server(ADDS) installed and click Start. After it started, double click on it to open</p>
<p align="center"><img src="https://i.imgur.com/HHdlLFJ.png" height="50%" width="50%" alt="image"/>

<p>2. Windows Setup opens up, click NEXT</p>
<p align="center"><img src="https://i.imgur.com/hVwZvvV.png" height="50%" width="50%" alt="image"/>

<p>3. On the next page, click INSTALL NOW</p>
<p align="center"><img src="https://i.imgur.com/RLY5EVf.png" height="50%" width="50%" alt="image"/>

<p>4. On the Select the Operating system you want to install page, selected Datacenter Evaluation(Desktop Experience) and click NEXT</p>
<p align="center"><img src="https://i.imgur.com/OjYk4zz.png" height="50%" width="50%" alt="image"/>

<p>5. On the Applicable notices and license terms page, check the “I accept the license terms” box, then click NEXT</p>
<p align="center"><img src="https://i.imgur.com/xqb1PE5.png" height="50%" width="50%" alt="image"/>

<p>6. On the Which type of installation do you want page, select “Custom: Install Windows only(advanced)”</p>
<p align="center"><img src="https://i.imgur.com/xRMTWQ3.png" height="50%" width="50%" alt="image"/>

<p>7. Next page shows the status of Installing windows</p>
<p align="center"><img src="https://i.imgur.com/YXsfTow.png" height="50%" width="50%" alt="image"/>

<p>8. After the installation, Administrator Password is required</p>
<p align="center"><img src="https://i.imgur.com/ZdVr8eO.png" height="50%" width="50%" alt="image"/>

<p>9. Next, you are asked to select a screen size, then connect</p>
<p align="center"><img src="https://i.imgur.com/9z9dXDi.png" height="50%" width="50%" alt="image"/>

<p>10. Then you asked to type in the Administrator’s password to log in</p>
<p align="center"><img src="https://i.imgur.com/anUzvp3.png" height="50%" width="50%" alt="image"/>

<br>

<h3>To rename the Computer</h3>
<p>1. Click on File and Folder, right click on this PC and click on Properties. This opens Control panel>system and security>system page. There, click on Advanced system settings. On the system properties’ page, select on the Computer name tab, then click Change. On the computer name/domain changes page, type in the Computer name and click OK</p>
<p align="center"><img src="https://i.imgur.com/jrc4HTn.png" height="50%" width="50%" alt="image"/>

<p>2. You are required to restart the computer to apply these changes, click OK</p>
<p align="center"><img src="https://i.imgur.com/sRE4rEx.png" height="50%" width="50%" alt="image"/>

<p>3. Click Restart Now</p>
<p align="center"><img src="https://i.imgur.com/rf7nBuS.png" height="50%" width="50%" alt="image"/>

<br>

<h3>To assign a unique IP address to the Windows 2019 Server(ADDS)</h3>
<p>1. Go to Network & Sharing Center on your computer. Then Ethernet. On the Ethernet status’ page, click on Properties, On the Ethernet Properties page, double click on Internet Protocol Version 4(TCP/IPv4) , select "Use the following IP address" and type in the IP Address, also select Use the following DNS server addresses and type it in.</p>
<p align="center"><img src="https://i.imgur.com/hAHrngI.png" height="50%" width="50%" alt="image"/>

<br>








<p align="center"><img src="" height="50%" width="50%" alt="image"/>
