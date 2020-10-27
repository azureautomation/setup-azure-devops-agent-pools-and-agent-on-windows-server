Setup Azure DevOps Agent Pools and Agent on Windows Server
==========================================================

            

This is sample code modified from DSC configuration to use used as a imperative script.


There are samples of:


1) Authenticating to Azure DevOps from PowerShell with a PAT token


2) Calling the api to test if the pool exists.


3) Creating the pool if it doesn't exist.


4) Downloading the Agent to the local Windows server


5) Testing to see if the agent is running


6) if the agent is not running, then it will install the agent into the pool.


 


Because this is just copied from a DSC Configuration, I tried to keep the $using: referenced that were used in the Script resource.


I just commented them out.


This is the sample code for creating the agents. Disclaimer, I have just copied my DSC configuration and Turned it into this powershell script..


**I did maintain idempotence within this script, so you can run it over and over again.**


 


Ensure you update your     orgUrl       = 'https://dev.azure.com/MyDevOpsOrg/'


Also update all of below:


 The meta data for defining the pools is here:  * this is part of the overall script.

 

        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
