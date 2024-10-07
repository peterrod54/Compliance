# Automated Compliance Reporting
Persistent cyber threats, plus the growing array of regulations & rapidly changing technology, have heightened the need for **_Compliance Reporting_** to be integrated into cybersecurity frameworks.

Yet, manually generating compliance reports is daunting, tedious and time-consuming. Automating the process is the way to go; it gives your organization a centralized, up-to-date view of your security posture, making compliance much more efficient. This automation ensures your reports adhere to major frameworks such as NIST, DISA, HIPAA, SOX, and PCI.  

Below are the steps required to install automated compliance reporting.

## Step 1
Get the **_download.zip_** file from the following file repository: [Google Docs](https://drive.google.com/file/d/12cd3b3yBbCkKTxQPhC9VpKvSl-wb0c3N/view?usp=sharing). (Note: **Right-Click link** and select **_Open Link in New tab_**)
#### File Hash Verification
**SHA256**: B627027A10F132796258B3A3D507F95D4C4C8E3E8CAC98CF025FFF793132CDAE 
#### Prerequisites
+ **Windows Server 2016 and above**
+ **Minimum 6 GB RAM**
+ **Minimum 2 CPUs**
+ **IIS or Apache Web Service**

       (Note: Installing and configuring the Web Service is beyond the scope of this project)

## Step 2
Once the file is extracted, move the "Compliance" directory to the root partition of your C: drive. Your directory structure should look like the following:

![image](https://github.com/peterrod54/Compliance/assets/57069647/6da2efbc-1b16-4db7-ac99-b96e59a20aa8)

## Step 3
Open the **_hosts.txt_** and enter the hostnames or IP addresses that you want to scan. Refer to the **_hosts_-_example.txt_** file to see how that's done.

**NOTE**: It takes approximately 6 minutes to scan one host.  I recommend that you keep your list of hosts to under 10, at least for your first scan.  After that, you can add more hosts to that list but remember that the more hosts you add, the longer the scan will take to generate the compliance report.

## Step 4

Right-Click _Invoke_Scan_ and **_Run as administrator_**

**Note:** Two things to keep in mind to successfully launch scan:
(1) Internet access is required.
(2) Launching the **_Invoke_Scan_** file requires elevated permissions.

## Step 5

Right-Click _IIS Manager_ and **_Run as administrator_** (_This Step assumes that you have installed and configured IIS Manager_)
+ Right-click "_Default Web Site_"
+ Select "_Add Virtual Directory_"
+ Configure virtual directory as follows:

  ![ComplianceHtmlReports](https://github.com/user-attachments/assets/4ff696ce-933a-46cb-89be-ddf0baef31a5)

+ Next, you'll want to create a share for the following directory **_C:\Compliance\Reports\HTML_** and provide the required Security settings and permissions.


### Where can I find the Compliance Report?
The _Compliance Report_ is generated as an Excel file (**XLSX**) and is located in the **C:\Compliance\Reports** directory.

### What you can expect your Excel report to look like:
![Compliance_Excel2](https://github.com/peterrod54/Compliance/assets/57069647/ff60449b-1d94-4f09-9740-22f7b7fc913f)

![image](https://github.com/peterrod54/Compliance/assets/57069647/66781262-6fea-479a-8575-4b1c3ed57e24)

![image](https://github.com/peterrod54/Compliance/assets/57069647/74423c72-f4e8-4ccf-80a8-07bfe132c54e)


### What you can expect the results of an single benchmark report to look like:
![Compliance_Report](https://github.com/peterrod54/Compliance/assets/57069647/7175933b-f1c1-4b68-b8eb-3745043b0055)

### Error Logs

An error log is generated after each scan. If you run into issues executing a compliance scan, this is where you'll want to look first. Error Logs are located in: **_C:\Compliance\Logs_**

# Final Thought
Once you've completed the above steps, contact me if you need further instructions, of if you're interested in how you can incorporate your compliance report into a _web-based_ reporting platform, such as SSRS, PowerBI, or similar platform (see example below). [Contact Me](mailto:peter@variacom.com)

![image](https://github.com/peterrod54/Compliance/assets/57069647/77b36f61-0950-4508-aaf8-2de182c25be2)

