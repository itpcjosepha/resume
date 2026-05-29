# Hearing Care Solutions (2022-2025) 
https://www.hearingcaresolutions.com | https://www.wsa.com/about/

# About WSA
One of the world's largest manufacturers of hearing aids and hearing healthcare solutions. Headquartered in Denmark and Singapore, the multinational company was formed in 2019. 

# Project Highlights:

• Developed a daily 7 million row ETL transfer from a 8 year old FileMaker Pro solution into MS SQL Server
• Implemented webhooks
• Implement SDLC environment for FileMaker files. DEV->QA->UAT->PROD. 
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


The focal FileMaker solution I created would extract, transfer, and load over 7million rows of data from backup files of the 8 year old FileMaker file to SQL Server. The screenshot of what I developed is headed in blue with “FM<=>SQL (Solution Analysis)”  the yellow card with redacted data is the original 8 year old program that I did not develop or design. 

The SQL Server screenshots is the FileMaker data in SQL Server after a ETL event. 

The program was created by reverse engineering the original FileMaker solution and scaffolding a new FileMaker file and essentially exported data from a daily backup and load it into SQL Server using SQL Server bulk import. 

Business goal was to allow the reporting team to use SQL Server and replace all internal FileMaker Pro reports that could take days to run on a production environment. We provided the ability to connect PowerBI and Sisense analytics & reporting.

Included are pictures of the database schema. I use the “Anchor-Buoy” methodology for FileMaker relationships, which means each table is represented one time with its own color and related tables. For a breakdown of this methodology this article is great: https://highpowerdata.com/three-models-for-the-filemaker-relationship-graph/ 
