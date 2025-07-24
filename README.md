<h1>Automated Intrusion Detection in Containerized Environments</h1>

<h2>Description</h2>
In Progress...
<br />

<h2>Technologies used</h2>

- <b>IDS tools: Snort, Suricata, Zeek, and Splunk</b> 
- <b>Attacks Techniques: Coming soon</b>

<h2>Environments Used </h2>

- <b>Docker Machine with multiple containers</b> (Target Machine)
- <b>IDS Machine</b> (Network Monitor)
- <b>Splunk</b> (Network Monitor)
- <b>Kali Linux</b> (Attacking Machine)
<h2>Project Documentation:</h2>
<b>In Progress...</b>
<p align="center">
Simulated environment on VMWare: <br/>

1. All testing is done within a controlled environment within VMWare where there are a total of four VMs used each with its own task.
a.	Target Machine – Docker/Containers <br/>
The Docker machine is going to be our target machine but as it will be configured with all of the containers we would be attacking them and not the actual machine itself. Each container simulates a different service or application might exist in a real production environment. The overall purpose of this machine is to replicate a real world containerized infracture where various threats can be tested against different services.<br/>
b.	Attacking Machine – Kali Linux<br/>
The Kali machine was where we conducted all of the attacks from. It comes with pre installed tools useful for penetration testing and other resources needed for test attacks against the containers. Metasploit, SQL map, and regular CLI<br/>
c.	IDS Machine – Snort, Suricata, Zeek (Ubuntu OS)<br/>
This system is configured with all three IDS. These tools will monitor network traffic flowing to and from the target machine. They are configured with the appropriate interfaces, rulesets, and logging paths. The Splunk forwarder is also installed and configured with the paths so the logs can be sent to Splunk and further analyzed there. The alerts and logs generated here are critical for identifying suspicious behavior and evaluating the detection efficacy. This VM played a key role in being able to identify and analyze the threats in real time<br/>
d.	SIEM Machine – Splunk (Ubuntu OS)<br/>
Splunk is installed and configured on this VM to collect, parse, and visualize logs and alerts from the IDS system. It acts as a log management and monitoring platform. By using forwarders the machine was able to get the ingested logs from Snort, Zeek, and Suricata. This enabled the creation of dashboards, alerts, and summaries that reflect the system activity.<br/>  
<br />
<br />
Figure 2: . <br/>
<img src="" height="80%" width="80%" alt="Project Steps"/>
<br/>
