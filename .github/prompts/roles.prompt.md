# Roles audit

You can find roles located at src/roles. 

There will be a folder per role.

Example: src/roles/*/role.yml.

I need help finding changes to this codebase that do not align with the following standards

- "Read only" - roles must only give prvRead permissions

- "User role" - roles do not give prvDelete permission. The following system permissions can be ignored: (prvDeleteNewProcess, prvDeleteTranslationProcess, prvDeleteUserApplicationMetadata, prvDeleteUserEntityUISettings, prvDeleteWorkflow, prvDeleteWorkflowSession)

[Back](Prompt.prompt.md)