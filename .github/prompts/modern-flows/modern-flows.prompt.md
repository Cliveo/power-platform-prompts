# Modern Flows

I need help finding changes to this codebase that do not align with the standards for modern flows.

You can find possible connection references to use in src/connectionreferences.

Flows can be found at src/modernflows/

You can find a reference to a good flow:
- [flow.json](dc1a19b9-00ed-ef11-be20-000d3ad0347e/Goodflow-DC1A19B9-00ED-EF11-BE20-000D3AD0347E.json)
- [workflow.yml](dc1a19b9-00ed-ef11-be20-000d3ad0347e/workflow.yml)

This flow is good because:
* It contains a meaningful description
* The trigger and every action have descriptive names instead of default values
* It uses filters when querying rows from Dataverse

You can find reference to a bad flow here:
- [flow.json](f867c020-60eb-ef11-be20-000d3ad0347e/HTTPnoauth-F867C020-60EB-EF11-BE20-000D3AD0347E.json)
- [workflow.yml](f867c020-60eb-ef11-be20-000d3ad0347e/workflow.yml)

This flow is bad because:
* It uses HTTP trigger with all auth type (HTTP can be used but it must be secured with minimum "Tenant" level)
* It's using a default connection reference (e.g. co_sharedcommondataserviceforapps_<random-suffix>). The connection reference should be in the format co_<Connection><Solution name> like, co_DataverseDemo
* The trigger and actions do not have meaningful names

[Back](../Prompt.prompt.md)