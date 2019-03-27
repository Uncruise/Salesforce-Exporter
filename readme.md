
Data Loader
https://help.salesforce.com/articleView?id=data_loader.htm

Exporter Setup Instructions

1) Install Git for Windows -> http://gitforwindows.org
    NOTE: Don't need to have an account just need the application installed

2) **501 Admin** will provider zip file for custom settings ([Client].zip).  Extract zip into C:\repo.  After unzip there should be a c:\repo\Salesforce-Exporter-Private directory

Example: C:\repo\Salesforce-Exporter-Private\Clients\XYZ where XYZ are the ClientInitials should contain an Exporter.bat file and a DataLoader directory.

3) Edit c:\repo\Exporter-Private\Exporter.bat
    Check & Verify the following values - update accordingly
    * EMAIL_LIST - include client emails
    * IMPORT_DIRECTORY - Location of incoming data files (e.g., DropBox, OneDrive)

Running Export

Run c:\repo\Salesforce-Exporter-Private\Exporter.bat to start the Exporter.  You can run
    - Exporter.bat manually
    - schedule with Task Scheduler (be sure to set working directory to the Exporter.bat directory)

Troubleshooting

1) [Short summary] 
Issue: 
Resolution: 
