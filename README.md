<h1>File Integrity Monitoring (FIM) using Wazuh</h1>



<h2>Description</h2>
This project focuses on implementing File Integrity Monitoring (FIM) using Wazuh to detect unauthorized changes in a public directory. The objective was to monitor modifications in a specific directory and track changes in real-time, enhancing security monitoring and incident response.<br/>


<br />

<h2>Tools Used</h2>

- <b>Wazuh Manager (SIEM & Security Monitoring)</b> 
- <b>Wazuh Agent (Installed on Windows 10 Client VM)</b>
- <b>Windows 10 VM (Test environment)</b>


<h2>Steps Undertaken :</h2>

  1. <b>Agent Installation:</b><br/>
     - Installed and configured the Wazuh Agent on a Windows 10 client VM.<br/>
     - Connected the agent to the Wazuh Manager.<br/>


     <img src="https://i.imgur.com/gxH4VdX.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
     
<br />
<br />
 2. <b>Configuration of ossec.conf:</b><br/>
     - Edited the ossec.conf file to specify the public directory to be monitored.<br/>
  

<img src="https://i.imgur.com/EUNBv3A.png" height="90%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

  3. <b>Monitoring Directory Changes:</b><br/>
     - Created a sample file named bank_account.txt in the public directory.<br/>
     - Modified the file to observe how Wazuh detects changes.<br/>
<img src="https://i.imgur.com/YhcHdvG.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/kmlrTJQ.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<br />
<br />
 4. <b>Updated the ossec.conf file to enable real-time monitoring of the specified directory.</b><br/>
     
<img src="https://i.imgur.com/frLEy59.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/NaBprqh.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<br />
<br />
5. <b>Enhancing Monitoring with 'who-data' and Report Changes Option</b><br/>
     - Configured who-data to capture user activity related to file modifications.<br/>
     - Enabled the "report_changes" feature in ossec.conf to track content changes.<br/>

  <br/>
<img src="https://i.imgur.com/gWhQvpw.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>

<br />

6. <b>Observing the Results:</b><br/>
     - Reviewed the alerts and logs in the Wazuh Dashboard to analyze changes and identify potential security incidents.<br/>
     

  <br/>
<img src="https://i.imgur.com/LzjS8Gf.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/s1EnYVH.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/bDOU1rL.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/jEXhk3Q.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>


<h2>Key Learnings</h2>
     - Understanding how Wazuh's File Integrity Monitoring (FIM) works.<br/>
     - Configuring ossec.conf to monitor specific directories and enable real-time alerts.<br/>
     - Utilizing who-data and report_changes to enhance monitoring capabilities.<br/>
     - Analyzing alerts and logs to detect unauthorized file modifications.<br/>


</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
