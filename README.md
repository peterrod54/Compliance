# Automated Cybersecurity Compliance Reporting

Automating cybersecurity compliance reports can play a pivotal role in adherence to industry regulations, providing organizations with a centralized and comprehensive view of their security posture, which can be shared with auditors and regulators.  Below are the steps required to install an automated cybersecurity compliance reporting infrastructure.

## Step 1

Download the **_Compliance.zip_** file from the following file repository: [Google Docs](https://drive.google.com/file/d/1Ffju4Wnxc0hrmKAjkW9kQNPQKEY3foCe/view?usp=sharing). (**_Note: Right-Click link and select new tab_**)

## Step 2

After download, extract file to the root partition (C:).  Once the file is extracted, your directory structure should look like the following:

![Compliance_Dir](https://github.com/peterrod54/Compliance/assets/57069647/1124a204-0884-408b-9b24-0f740e957ccc)

## Step 3

Open the **_hosts.txt_** and enter the hostnames or IP addresses that you want to scan. Refer to the **_hosts_-_example.txt_** file to see how that's done.

**NOTE**: It takes 6 minutes to scan one host.  I recommend that you keep your list of hosts to under 10, at least for your first scan.  After that, you can add more hosts to that list but remember that the more hosts you list in the text file, the longer the scan will take to generate the compliance report.

## Step 4

Launch **_VCS-Scanner.exe_** 

Two things to keep in mind:
    1. Internet access is required.
    2. Launching executable requires elevated permissions.
