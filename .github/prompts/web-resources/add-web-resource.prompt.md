# Add Web resource

## Context

You have been asked to add a web resource to this repo.

First ask the user what the webResourceName of the web resource will be. A good name usually be in the format co_Contact_Form or co_Contact_Ribbon.

Generate a random guid for the web resource

Add a row in rootcomponents.yml like
- '@type': 61
    '@schemaName': co_webResourceName
    '@behavior': 0


Add a row in solutioncomponents.yml like
- '@path': /webresources/55a4bea9-aaec-ef11-be20-000d3ad0347e

You need to create a folder in src/webresources using the random guid

Replace everything from the sample where you find 55a4bea9-aaec-ef11-be20-000d3ad0347e with the random guid for our new web resource

Add the following files in the new folder you created
Make sure that the web resources file has everything like this [yaml](55a4bea9-aaec-ef11-be20-000d3ad0347e/webresource.yml)
And provide a sample using [javascript](55a4bea9-aaec-ef11-be20-000d3ad0347e/co_webResourceName55A4BEA9-AAEC-EF11-BE20-000D3AD0347E.js)

then prompt the user to run command git sync

[Back](../Prompt.prompt.md)