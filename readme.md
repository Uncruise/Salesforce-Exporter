
Data Loader
https://help.salesforce.com/articleView?id=data_loader.htm

Setup Instructions

1) Install Zulu & Salesforce Data Loader (Instructions -> https://help.salesforce.com/articleView?id=loader_install_windows.htm)

2) Install the latest Java Platform (JDK) -> https://www.oracle.com/technetwork/java/javase/downloads/index.html 

3) Install Git for Windows -> http://gitforwindows.org
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

1) [Short summary] 
Issue: 
Resolution: 
