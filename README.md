# DataManagerExports

Each Module should have it's own folder.

###Agency Exports and Folder Structure###
Agency exports should be built inside the Module folder it was created in.  The folder should be named as the full agency name and not the serv prov code for better searchibility. The main export that should be in these folders should be the record types for that agency for that module.  You can export all record types for that module or organize by having single exports for each record type.  Each folder should also have a README.md file which describes the records included.

###Standard Base###
The standard base is the initial configuration that should be set up from day one of every project.  It includes the following areas:
1.	Standard Choices – the standard choices import includes 300+ already created SCs, including descriptions and pre-populated best practice data.  These are built with the most commonly turned on features and setup. There is also an ad hoc report build that will take the metadata of the standard choice descriptions and align them by subject, so you can see what belongs to inspections or workflow for example.  This is done by tagging inside the description.
2.	Form Portlet Designs – this import includes designed forms, following best practice design, for over 700 forms and lists.  Each one includes the proper naming conventions, alignment and spacing.  
3.	ACA General Form Design – this import cleans up the forms for the general areas of ACA.  This is mainly around registration and contacts.
4.	Agency Menu structure – this import is a standard menu structure so the agency has a starting template.
5.	Standard Consoles – consoles have been created as starting points for standard roles such as admin, staff, asset management and inspectors. Each one is designed to give the user a properly built console instead of starting from scratch. Note, you must add security permissions to these once you create your user groups.
6.	Standard Saved Searches – initial saved searches have been added as a starting point for agencies.  These include My Inspections, My Records, My Tasks, Submitted Online, and Today’s Records.  These are considered the most often used saved searches.  Note, you must add security permissions to these once you create your user groups.
7.	Notification Templates – the most often used notification templates have been built and given naming properties so they can be easily found.  Now you have starting content with these notificiations.
8.	Events – all events that have a standard master script are now set up with this import file.  These are the most often used scripts and events.
