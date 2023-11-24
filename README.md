# Automated Cybersecurity Compliance Reporting
Automating cybersecurity compliance reports can play a pivotal role in adherence to industry regulations, and provide organizations with a centralized and comprehensive view of their security posture, which can be shared with auditors and regulators.  Below are the steps required to install an automated cybersecurity compliance reporting infrastructure.

## Step 1
Download the **_Compliance.zip_** file from the following file repository: [Google Docs](https://drive.google.com/file/d/18m5NfWfAevqH8KBHJ431g1FQcjCXVCQA/view). (**_Note: Right-Click link and select new tab_**)
#### File Hash Verification
**SHA256**: 9B9609A35368A600F343E27376FDCB1C216B03A7646D7F9F5BBDC3D497330C85 
#### Prerequisites
+ Windows Server 2016 and above
+ Minimum 6 GB RAM
+ Minimum 2 CPUs

## Step 2
Extract downloaded file to the root partition (C:).  Once the file is extracted, your directory structure should look like the following:

![Compliance_Dir](https://github.com/peterrod54/Compliance/assets/57069647/1124a204-0884-408b-9b24-0f740e957ccc)

## Step 3
Open the **_hosts.txt_** and enter the hostnames or IP addresses that you want to scan. Refer to the **_hosts_-_example.txt_** file to see how that's done.

**NOTE**: It takes 6 minutes to scan one host.  I recommend that you keep your list of hosts to under 10, at least for your first scan.  After that, you can add more hosts to that list but remember that the more hosts you add, the longer the scan will take to generate the compliance report.

## Step 4
Launch **_VCS-Scanner.exe_** 

Two things to keep in mind to successfully launch app:
(1) Internet access is required.
(2) Launching the executable requires elevated permissions.

### Where can I find the Compliance Report?
The _Compliance Report_ is generated in the **_C:\Reports_** directory.

### What you can expect your Excel report to look like:
![Compliance_Excel2](https://github.com/peterrod54/Compliance/assets/57069647/ff60449b-1d94-4f09-9740-22f7b7fc913f)




### What you can expect your benchmark reports to look like:
![Compliance_Report](https://github.com/peterrod54/Compliance/assets/57069647/7175933b-f1c1-4b68-b8eb-3745043b0055)



# Final Thought
You may experience an issue with your antimalware preventing the execution of the _**VCS-Scanner**_ app. If so, you'll need to add that app to the antimalware white-list. If adding the app to a white-list doesn't resolve the issue, please make the effort to resolve the issue yourself.  If you still need help let me know. [Email me](mailto:peter@variacom.com)
