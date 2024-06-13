# Automated Cybersecurity Compliance Reporting
Tired of manually generating compliance reports? Automating the process gives your organization a centralized, up-to-date view of your security posture, making compliance much more efficient. This automation ensures your reports adhere to major frameworks like HIPAA, SOX, and PCI.  Below are the steps required to install an automated cybersecurity compliance reporting infrastructure.

## Step 1
Get the **_download.zip_** file from the following file repository: [Google Docs](https://drive.google.com/file/d/17Oq_zRMbcevm0gGnoUh8kSIk5mPe0ydl/view?usp=sharing). (**_Note: Right-Click link and select new tab_**)
#### File Hash Verification
**SHA256**: 8D5AD9F80D5236B043CA9527E9B21C7A14727CD5B45BCEB29B47B86E29722775 
#### Prerequisites
+ Windows Server 2016 and above
+ Minimum 6 GB RAM
+ Minimum 2 CPUs

## Step 2
Once the file is extracted, move the "Compliance" directory to the root partition of your C: drive. Your directory structure should look like the following:

![image](https://github.com/peterrod54/Compliance/assets/57069647/6da2efbc-1b16-4db7-ac99-b96e59a20aa8)

## Step 3
Open the **_hosts.txt_** and enter the hostnames or IP addresses that you want to scan. Refer to the **_hosts_-_example.txt_** file to see how that's done.

**NOTE**: It takes 6 minutes to scan one host.  I recommend that you keep your list of hosts to under 10, at least for your first scan.  After that, you can add more hosts to that list but remember that the more hosts you add, the longer the scan will take to generate the compliance report.

## Step 4

Once you have added the hosts that you want to scan, run the **_Invoke_Scan_** executable

Two things to keep in mind to successfully launch app:
(1) Internet access is required.
(2) Launching the **_Invoke_Scan_** executable requires elevated permissions.

### Where can I find the Compliance Report?
The _Compliance Report_ is generated in the **_C:\Compliance\Reports_** directory.

### What you can expect your Excel report to look like:
![Compliance_Excel2](https://github.com/peterrod54/Compliance/assets/57069647/ff60449b-1d94-4f09-9740-22f7b7fc913f)

![image](https://github.com/peterrod54/Compliance/assets/57069647/66781262-6fea-479a-8575-4b1c3ed57e24)

![image](https://github.com/peterrod54/Compliance/assets/57069647/74423c72-f4e8-4ccf-80a8-07bfe132c54e)


### What you can expect the results of an single benchmark report to look like:
![Compliance_Report](https://github.com/peterrod54/Compliance/assets/57069647/7175933b-f1c1-4b68-b8eb-3745043b0055)



# Final Thought
Once you've completed the above steps, contact me for further instructions. [Email me](mailto:peter@variacom.com)
