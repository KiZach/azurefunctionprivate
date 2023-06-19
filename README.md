# Infrastructure deployment

This part of the project is the Azure infrastructure componets needed to run the an internal Azure function.

Currently the infrastructure has these components:

- VNET
- Subnets
- ...

## Deploy Bicep template

To deploy the infrastructure directly from code use the following commands:

- Connect-AzAccount -Tenant xyz
- Set-AzContext -Subscription xyz
- New-AzSubscriptionDeployment -Name LocalPSDeployment -Location westeurope -TemplateFile ./infrastructure/deploy.bicep

To deploy the code you must have at least contributor access to the Azure subscription above.
