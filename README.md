# Automated Cybersecurity Compliance Reporting
Automating compliance reporting replaces the manual and cumbersome process of providing organizations with an efficient, centralized and comprehensive view of their security posture; this automated compliance reporting process adheres to major compliance frameworks, such as HIPPA, SOX, PCI and others.  Below are the steps required to install an automated cybersecurity compliance reporting infrastructure.

## Step 1
Get the **_download.zip_** file from the following file repository: [Google Docs](https://drive.google.com/file/d/1PnB91vmkpOs2dJCzoNMVpI73uGTzj1Rn/view?usp=sharing). (**_Note: Right-Click link and select new tab_**)
#### File Hash Verification
**SHA256**: 85327DC9B03366284DCC1C91EDD6F7CF658BAAB83F6A7D261B1D58C84CBE10B2 
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


### What you can expect your benchmark reports to look like:
![Compliance_Report](https://github.com/peterrod54/Compliance/assets/57069647/7175933b-f1c1-4b68-b8eb-3745043b0055)


# Final Thought
Once you've completed the above steps, contact me for further instructions. [Email me](mailto:peter@variacom.com)
