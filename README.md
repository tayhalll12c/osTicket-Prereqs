<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This demonstration outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Windows 10 Virtual Machine with 2-4 Virtual CPUs 
- Installation of Windows IIS with CGI
- Installation of PHP Manager for IIS
- Installation of additional PHP files 
- Installation of MySQL 5.5.62
- Installation of HeidiSQL
- Setup of osTicket in browser 

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/iCIyqzo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In Azure, create a Windows 10 virtual machine wich 2-4 virtual CPUs. 
</p>
<br />

<p>
<img src="https://i.imgur.com/kJ0D4bB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Inside the virtual machine, open control panel, navigate to the features panel, and check the IIS box. 
</p>
<br />

<p>
<img src="https://i.imgur.com/hnyN1PU.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Use the dropdown boxes to navigate to CGI, and enable it. This is necessary for the installation of PHP manager. Then, click the 'OK' button. 
</p>
<br />

<p>
<img src="https://i.imgur.com/0ojkvxH.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install PHP manager.  
</p>
<br />

<p>
<img src="https://i.imgur.com/WfaJXxK.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install 'rewrite' module.  
</p>
<br />

<p>
<img src="https://i.imgur.com/ZfnK7bi.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a new folder in the C: drive titled "PHP" 
</p>
<br />

<p>
<img src="https://i.imgur.com/vpcWebt.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install PHP 7.3.8 files and extract contents into PHP folder that was created in C: drive  
</p>
<br />

<p>
<img src="https://i.imgur.com/4IO4z8i.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install Microsoft Visual C++ Redistributable.
</p>
<br />

<p>
<img src="https://i.imgur.com/nJFHrQa.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open MySQL 5.5 setup wizard.  
</p>
<br />

<p>
<img src="https://i.imgur.com/sfX4tN9.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select the 'Typical' installation box.   
</p>
<br />

<p>
<img src="https://i.imgur.com/TyfgV7B.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click 'Finish' and launch the MySQL Instance Configuration Wizard.   
</p>
<br />

<p>
<img src="https://i.imgur.com/jGasxIh.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Configuration Wizard, select 'Standard Configuration'.   
</p>
<br />

<p>
<img src="https://i.imgur.com/E9JDFQ1.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install as Windows Service.    
</p>
<br />

<p>
<img src="https://i.imgur.com/G24ZpES.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Type in a password that you will remember later.     
</p>
<br />

<p>
<img src="https://i.imgur.com/ZOmJgs2.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select 'Execute' and finish the Configuration.      
</p>
<br />

<p>
<img src="https://i.imgur.com/MkahFnx.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Run IIS as an administrator.      
</p>
<br />

<p>
<img src="https://i.imgur.com/1ZGhjQw.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click 'PHP Manager'.      
</p>
<br />

<p>
<img src="https://i.imgur.com/eMvduh5.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click 'Register new PHP version'.       
</p>
<br />

<p>
<img src="https://i.imgur.com/kjRCfOL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Provide a path to php-cgi executable.       
</p>
<br />

<p>
<img src="https://i.imgur.com/IDctCkg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Make sure the name of the server is highlighted, and then click 'Restart'.       
</p>
<br />

<p>
<img src="https://i.imgur.com/Fnd7otC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install osTicket file.       
</p>
<br />

<p>
<img src="https://i.imgur.com/SfhuGjl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Inside the osTicket file, drag its 'upload' folder into the following destination: C:> inetpub> wwwroot       
</p>
<br />

<p>
<img src="https://i.imgur.com/FH2fnHm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Rename 'upload' folder to "osTicket".      
</p>
<br />

<p>
<img src="https://i.imgur.com/0hfnQUp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Restart the server again.       
</p>
<br />

<p>
<img src="https://i.imgur.com/mGMOdNj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Under the dropdown menu, click 'osTicket' and then click 'Browse *:80'.      
</p>
<br />

<p>
<img src="https://i.imgur.com/mBzUGV7.png" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
This page will appear in a browser. Some extensions are still required in order to ensure full functionality of osTicket.       
</p>
<br />

<p>
<img src="https://i.imgur.com/HDlMog2.png" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click 'PHP Manager' in osTicket Home.       
</p>
<br />

<p>
<img src="https://i.imgur.com/THWevYr.png" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click 'Enable or disable an extension'.       
</p>
<br />

<p>
<img src="https://i.imgur.com/IMvHx05.png" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enable 'php_imap.dll'.       
</p>
<br />

<p>
<img src="https://i.imgur.com/usqTeQk.png" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enable 'php_intl.dll'.       
</p>
<br />

<p>
<img src="https://i.imgur.com/0jdWVvH.png" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enable 'php_opcache.dll'.       
</p>
<br />

<p>
<img src="https://i.imgur.com/wW3M9CY.png" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Refresh osTicket in browser and observe changes.        
</p>
<br />

<p>
<img src="https://i.imgur.com/BFPFW8c.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the following destination, select this file.         
</p>
<br />

<p>
<img src="https://i.imgur.com/NnyIRgp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Rename the file to remove the word "sample".          
</p>
<br />

<p>
<img src="https://i.imgur.com/xoTbK8R.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
In security properties for the file, click 'Advanced'.           
</p>
<br />

<p>
<img src="https://i.imgur.com/z3gUJJB.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click 'Disable Inheritance' and 'Remove all inherited permissions'.            
</p>
<br />

<p>
<img src="https://i.imgur.com/Q6BugTD.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click 'Add'.             
</p>
<br />

<p>
<img src="https://i.imgur.com/CrXqXKg.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click 'Select a principal', type "everyone" in the object name bar, click 'Check Names' and then click 'OK'.             
</p>
<br />

<p>
<img src="https://i.imgur.com/F96vVcQ.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
Check the 'Full control' box and then click 'OK'.              
</p>
<br />

<p>
<img src="https://i.imgur.com/A71yZUl.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click 'Apply'.              
</p>
<br />

<p>
<img src="https://i.imgur.com/RL0GvQK.png" height="90%" width="90%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click 'Continue' on the osTicket website.              
</p>
<br />

<p>
<img src="https://i.imgur.com/BSP55qs.png" height="90%" width="90%" alt="Disk Sanitization Steps"/>
</p>
<p>
Type in a helpdesk name and email. In this case, both are samples.               
</p>
<br />

<p>
<img src="https://i.imgur.com/eWRklBM.png" height="90%" width="90%" alt="Disk Sanitization Steps"/>
</p>
<p>
Type in the remaining credentials. (image contains samples)               
</p>
<br />

<p>
<img src="https://i.imgur.com/Y4sFwAg.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install HeidiSQL which in this case acts as a database client.                
</p>
<br />

<p>
<img src="https://i.imgur.com/i6EFWrx.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click 'New'.                 
</p>
<br />

<p>
<img src="https://i.imgur.com/kWBxEMf.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p>
<p>
Type in the credentials from the MySQL configuration wizard from earlier. In this case, the username is "root" and whichever password was created. Then, click 'Open'. </p>
<br />

<p>
<img src="https://i.imgur.com/qIxNeI9.png" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Add the username and password on the osTicket installation page. 
</p>
<br />

<p>
<img src="https://i.imgur.com/Q9b2hif.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Right-click 'Unnamed', hover over 'Create new' and then click 'Database'. 
</p>
<br />

<p>
<img src="https://i.imgur.com/Z3A6mLn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Name the database "osTicket" and then click 'OK'.  
</p>
<br />

<p>
<img src="https://i.imgur.com/I0mv1Lk.png" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
Type the database name "osTicket" and then click 'Install Now'   
</p>
<br />

<p>
<img src="https://i.imgur.com/crtCPz4.png" height="100%" width="100%" alt="Disk Sanitization Steps"/>
</p>
<p>
osTicket has been installed.    
</p>
<br />

<p>
<img src="https://i.imgur.com/1pGbVau.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Delete the folder titled "setup" in the following destination.     
</p>
<br />

<p>
<img src="https://i.imgur.com/Ysev6rD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Re-open properties for the 'ost-config' file that was previously renamed.   
</p>
<br />

<p>
<img src="https://i.imgur.com/UEuf1B1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click 'Edit' in advanced security settings while 'Everyone' is selected.   
</p>
<br />

<p>
<img src="https://i.imgur.com/CHXX45A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Change the permissions to only allow 'Read' and 'Read & Execute' and then apply the changes.   
</p>
<br />
