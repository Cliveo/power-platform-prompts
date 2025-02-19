# Add Web resource event

## Context

main forms can be found at */formxml/main/systemform.yml

give the user a list of main forms to update under each table, then ask them which js library and function name they want to add and then if its on load or on save.

then add this to the forms requested

formLibraries:
    Library:
    '@name': co_Monica_Form
    '@libraryUniqueId': '{c05826aa-613f-4ae4-b6c3-9c5eedb2cf04}'
events:
    event:
    '@name': onload
    '@application': false
    '@active': false
    Handlers:
        Handler:
        '@functionName': MonicaForm.formOnLoad
        '@libraryName': co_Monica_Form
        '@handlerUniqueId': '{e1298d5f-c58f-4a4d-8ea0-365a57edeceb}'
        '@enabled': true
        '@parameters': ''
        '@passExecutionContext': true

then prompt the user to run command git push 

[Back](../Prompt.prompt.md)