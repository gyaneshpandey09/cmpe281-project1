# cmpe281-project1
Web Application to upload/download/delete files using AWS technologies.

Professor: Sanjay Garje 
ISA: Divyankitha Urs 
Student: Gyanesh Pandey

Introduction: iBOX Web-App allows users to upload your files to an AWS S3 bucket.

Techstack: PHP7 with AWS SDK, hosted on AWS EC2.

This project uses the following AWS resources: 
EC2: Web servers. 
ELB: Distributes the requests among the active EC2. 
AutoScaling Group:	Create new instances if CPU average go over 80%. It is using a Launch Configuration based on a custom EC2 image created especially for this application. 
Single AZ RDS:	MySQL database. 
CloudFront:	Used for caching static content 
S3:	File Storage destination 
Transfer Acceleration:	Used for faster photo upload if user selected that option during upload. 
R53:	DNS for the application domain (www.bcartmedia.com) 
