# Mandiant Managed Defense

## Managed Hunting for Microsoft Defender for Endpoint

The Managed Hunting service leverages [Azure Lighthouse](https://docs.microsoft.com/en-us/azure/lighthouse/overview) to ingest data from the customer-owned event hub.
The following button deploys the Azure Resource Management template [azuredeploy.json](azuredeploy.json). The intent of the ARM template is to delegate the contributor role for the subscription containing the event hub to a Mandiant Managed Defense user group. Mandiant administrators from the user group will then configure the Managed Hunting service to ingest data from the customer-owned event hub.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Ffireeye%2Fmandiant_managed_hunting%2Fmain%2Fazuredeploy.json)

Subcription Owner role is required to complete the process triggered by the button.
