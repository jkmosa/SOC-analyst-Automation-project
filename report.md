
# SOC (Security operation center) automation project

## Author

- Mussie Shifera Assefa



**Step 1**

Visualization design using drawio
![Visual diagram](/images/simulated_lab_diagram.drawio.svg)

**Step 2**

Component setup (on prem)



What is sysmon?

System Monitor (Sysmon) is a Windows system service and device driver that, once installed on a system, remains resident across system reboots to monitor and log system activity to the Windows event log. It provides detailed information about process creations, network connections, and changes to file creation time.

Downloading sysmon for windows 10 and download the configuration from *[here](https://github.com/opafhartong/sysmon-modular/blob/master/sysmonconfig.xml)*.

After downloading both the files. Extract the sysmon compressed folder and make sure the config file is inside the extracted folder. open a powershell as administrator and change the current working directory to extracted folder and run the Sysmon64.exe bit executable file simple because the processor is 64-bit architecture. 

![sysmon](/images/sysmon_files.png)

use the 'i' option to install configuration files.

![sysmon_install](/images/sysmon_installation.png)




**Step 3**

Configure a server and endpoint to talk to one another.

**Step 4**

Generate a telemetry related to mimik cat on the endpoint and then trigger on wasa.

**Step 5**

Setup SOAR and integrate everything together (wasa, hive and shuffle)

## Wazuh [SIEM(security information and event managment) & XDR (extursion detection system)]

- Trigger alerts & perform response action


## Hive [case managment]

- Send email and responsive action to be decided by (SOC analyst)


## Shuffle [SOAR (Security Orchestration, Automation, and Response) capabilities]

- Receive wazuh alerts & send responsive actions


## Refference

