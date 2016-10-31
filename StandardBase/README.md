#DRIVE Foundations Deployment Guide
The DRIVE Foundations includes the following baseline configurations: 
•	Standard Choices – all standard choices preconfigured with categorized ad hoc reports to view configuration
•	Master Scripts 3.0 – all foundations and events using the productized Master Scripts 3.0 (v 8.0.1+)
•	Form Portlet Designs – all Agency level forms have been preconfigured with a standard format
•	ACA Form Designs – preconfigured ACA form and page designs
•	Consoles – standard consoles for common personas
•	Notification Templates – preconfigured notification templates for ACA and other notifications
•	Saved Searches – common saved searches for Record List, My Task List, Inspections, etc
•	Agency Menu – preconfigured agency level menu designs

All of the data manager export files for project drive are located on GitHub.
https://github.com/Accela-Inc/DataManagerExports/tree/master/StandardBase

 
#Standard Choices
This package will create every standard choice available in the platform with descriptions to help understand the use of each system switch and tags to organize them by features. This package will also deploy a series of ad hoc reports that can be used to view all of the standard choices associated with each feature.
This package can be imported into existing environments, including BPT environments. First you will import the data manager package with Reject ON. Then you will execute a batch job that will populate the descriptions for all existing standard choices.
See the “Import_Standard_Choice_Baseline_With_AdHocReports.docx” document for detailed instructions for importing the standard choices with ad hoc reports.


 
#Master Scripts 3.0
This package will install Master Scripts 3.0 using the productized version of the master scripts. This means that the master scripts and includes files will NOT exist under AA Classic > Events > Scripts. 
•	INCLUDES_ACCELA_GLOBALS & INCLUDES_ACCELA_FUNCTIONS now exist under AA Classic > Events > Master Scripts 
•	INCLUDES_CUSTOM now exists under AA Classic > Events > Custom Script
•	If you are deploying this into an existing environment
o	Copy all functions from Scripts > INCLUDES_CUSTOM into the Events > “Custom Script”
o	Delete the Scripts > INCLUDES_ACCELA_FUNCTIONS, INCLUDES_ACCELA_GLOBALS and INCLUDES_CUSTOM (to avoid confusion

#Instructions

1.	Import the data manager file: Master_Script_v3_Base_Standard_exportData.zip
o	Override:  ON
2.	Validate Standard Choice: EMSE_EXECUTE_OPTIONS
o	Value: SCRIPTS > Active
o	Value: STD_CHOICE > Inactive (for new environments, may be active for hybrid)
3.	Validate Standard Choice: MASTER_SCRIPT_DEFAULT_VERSION
o	Value: 8.0.1.0.0
Back Office Form Designs
This package contains preconfigured back office Agency level form designs.
Instructions
1.	Import the data manager file: Form_Portlet_Designs_Base_Stan_exportData.zip
a.	Override ON
2.	Verify the import was successful. You should now see “Form Name: XYZ” at the bottom of each form in the UI.
 
#ACA General Form Designs
This package contains preconfigured General ACA form designs.  
Instructions
1.	Import the data manager file: ACA_General_Form_Design_Base_exportData.zip
a.	Override ON
2.	Verify the import was successful. You should now see “Form Name: XYZ” at the bottom of each form in the UI.
Saved Searches
This package contains preconfigured Saved Searches.  
Instructions
1.	Import the data manager file: Standard_Saved_Searches_Base_exportData.zip
a.	Override ON
2.	The following saved searches are included:
a.	Task Dashboard: 
i.	My Activities
ii.	My Inspections
iii.	My Workflow Tasks
b.	Record List:
i.	My Records
ii.	Submitted Online
iii.	Today’s Records
c.	Inspections List:
i.	My Inspections

#Agency Menu
This package contains preconfigured menu for the Record Detail tabs.  
Instructions
1.	Import the data manager file: Agency_Menu_Base_Standard_exportData.zip
a.	Override ON
2.	Verify import was successful. 

#ACA Notification Templates
This package contains preconfigured notification templates for built in ACA notifications.  
Instructions
1.	Import the data manager file: Notification_Templates_Base_exportData.zip
a.	Override ON
2.	Verify import was successful. 

#Agency Console Configuration
This package contains preconfigured consoles at the Agency level.  This import is not required when deploying DRIVE onto a BPT environment.
•	Admin Default
•	AMS Default
•	Daily Default
•	Inspector Default
Instructions
1.	Import the data manager file: Notification_Templates_Base_exportData.zip
a.	Override ON
2.	Verify import was successful
