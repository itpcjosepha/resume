Hearing Care Solutions (2022-2024)

Project Highlights:

• Reverse engineer a 8 year old FileMaker Pro solution and transfer data to MS SQL Server with a orchestrated ETL process from daily backups.
• Implement SDLC environments. DEV->QA->UAT->PROD. 
• Ensure development would comply with HIPAA
• Implement SDLC controls for HiTrust certification.  
	
	Technology Stack:
		• SQL Server
		• ODBC / Linked Server to FileMaker Server
		• PowerShell
		• BulkLoad XSLT CSV 
		• Export All
		• Export Modified
		• FileMaker Server Admin API
		• External oAuth secure login implementation


The FileMaker solution I created for "Hearing Care Solutions” would; extract, transfer, and load over 7million rows of data from FileMaker to SQL Server. The screenshot of what I developed is headed in blue with “FM<=>SQL (Solution Analysis)”  the yellow card with redacted data is the original program that I did not develop or design. 

The SQL Server screenshots is the FileMaker data in SQL Server after a ETL event. The program was created by reverse engineering the original FIleMaker solution and scaffolding a FileMaker file to it and essentially extracts the daily backup data and loads it into SQL Server. This was done to allow the reporting team to connect PowerBI and Sisense analytics & reporting to FileMaker data without having to use FileMaker. 

Included are pictures of the database schema. I use the “Anchor-Buoy” methodology for FileMaker relationships, which means each table is represented one time with its own color and related tables. Here is a breakdown of the different methods https://highpowerdata.com/three-models-for-the-filemaker-relationship-graph/ 
