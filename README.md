Automated ATT&CK Defense: Sysmon & Azure Integration 

# Project Proponent
Name: Kaushikq Ravindran <br />
Program: Masters in Software Engineering <br />
Institution: San Jose State University <br />
Portfolio: https://kaushikq-ravindran.github.io

# Project Scope
This project provides a detailed exploration of deploying and managing Azure Sentinel, an advanced SIEM system, integrated with Sysmon data collection, all within an automated infrastructure provisioned using Terraform. It simulates a security operations workflow for detecting, investigating, and responding to cyber threats.

# Technical Deployment Steps
### Resource Group Creation: 
Set up a designated Azure resource group with a specific naming convention, ensuring compatibility with Azure Sentinel requirements.
###  ARM Template Deployment: 
Utilize the azuredeploy.json for deploying the Sentinel-ATT&CK architecture automatically. Adjust the signedExpiry parameter within the SAS token properties to ensure proper whitelisting functionality and data security.
###  Whitelist Configuration: 
Populate the Azure Blob storage container with the necessary whitelisting files from the lab/files directory to filter and manage the Sysmon log data effectively.
###  Lab Environment Provisioning: 
Execute the Terraform script to establish a virtual lab environment where virtual machines are pre-configured with the Sysmon agent and the customized Sysmon configuration file.
###  Sysmon Data Integration: 
Implement the Sysmon log parser to structure the log data according to the OSSEM model, enabling effective ingestion into Azure Sentinel for threat detection and hunting exercises.

# Cost Management Strategies
The project incurs a monthly cost of approximately $125, mainly due to VM and storage utilization.
Implement cost-saving measures by de-provisioning the lab environment when inactive and re-provisioning as needed for class sessions or individual study.

# Educational Outcomes
Gain practical experience in deploying a cloud-native SIEM solution and integrating endpoint security data.
Develop skills in using infrastructure as code for cybersecurity applications.
Understand the application of MITRE ATT&CK framework in a live security monitoring system.
