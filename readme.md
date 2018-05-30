
Data Loader Guide
http://resources.docs.salesforce.com/210/17/en-us/sfdc/pdf/salesforce_data_loader.pdf

Data Loader Quick Reference
http://www.developerforce.com/media/Cheatsheet_Setting_Up_Automated_Data_Loader_9_0.pdf

Setup Instructions

1) Install Salesforce Data Loader (Instructions -> https://help.salesforce.com/articleView?id=000239784&type=1)

NOTE:
  a) Make sure your current user has Administrator access on the machine
  b) During Installation on the 'Install for admins only?' screen when prompted for 'Do you have administrator rights on this machine?' select Yes

2) Run Salesforce Data Loader to verify installation.  If you need Java installed then you will be prompted to install Java and follow the process to install Java. After Java installed run Data Loader to verify installation. 

3) Install Git for Windows http://gitforwindows.org
    NOTE: Don't need to have an account just need the application installed

4) Install Python 2.7.14 https://www.python.org/downloads/ 

5) **501 Admin** will provider zip file for custom settings ([Client].zip).  Extract zip into C:\repo\Salesforce-Exporter-Private\Clients\[Client].

Example: C:\repo\Salesforce-Exporter-Private\Clients\XYZ where XYZ are the ClientInitials should contain an Exporter.bat file and a DataLoader directory.

6) Edit c:\repo\Exporter-Private\Exporter.bat
    Check & Verify the following values - update accordingly
    * EMAIL_LIST - include client emails
    * IMPORT_DIRECTORY - Location of incoming data files (e.g., DropBox, OneDrive)
    * JAVA_HOME - Verify directory is valid or change to correct xxx version number based on installed C:\Program Files\Java\jre1.8.0_xxx\bin

Running Export

Run c:\repo\Exporter-Private\Exporter.bat to start the Exporter.  You can run
    - Exporter.bat manually
    - schedule with Task Scheduler (be sure to set working directory to the Exporter.bat directory)

Troubleshooting

1) Salesforce Data Loader can't install Admin version to C:\Program Files (x86)\salesforce.com
Resolution: You can install on another machine where you are an administrator and then just copy the salesforce.com directory to C:\Program Files (x86) to your target machine.
