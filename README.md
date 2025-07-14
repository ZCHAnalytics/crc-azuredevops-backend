# crc-azuredevops-backend

1. Create azure subscription for development stage of azure devops
2. Create new project in Azure DevOps organization called cloud-resume
3. Create repositories for backend and frontend
4. push existing code form VSC to repositories
   git remote set-url origin <>
   git push -u origin --all

5. store service principal credentials in Azure DevOps pipeline varialbes (secrets)

A. Create new client secret
Azure portal > App registrations > SP > Manage > Certificate & Secrets > New > copy value immediately 
value
secret id 
project > project settings > service connections > Azue Resource Manager > App registration (manual) > Credential (secret) > Credential (service [rincipal key
From azure portal app registration > overviedw > directory (tennat) ID copy and paste
   - keeping the same storage account for visitor  count
az ad app list --query "[?createdDateTime >= '2025-07-01' && createdDateTime < '2025-08-01'].{Name:displayName, AppId:appId, Created:createdDateTime}" --output table

6. Creat depliy backnedn ifnra yml
7. instlal terraform extension by Microsfot DEvlabs on the marketpalce
8. 
create new pipeline > Azure Repo > cloud-resume-backend > existing Azure Pipelines yaml file > path > continue > run
