# Non-functional requirements

I need help finding changes to this repo that do not align with the standards for nonfunctional requirements.

## Context

Aliases with preferred name on the left and schema name on the right:
- Table = Entity
- Column = Attribute

Each entity is in a folder in src/entities.

Example: src/entities/*/entity.yml

Responding by going through each entity would be best.

If you find the entity is unmodified (unmodified: 1). You can skip it. Let the user know you are skipping it because it's uncustomized.

## Requirement

If you find metadata in the entity containing these settings:
- IsAuditEnabled: 0
- IsRetrieveAuditEnabled: 0
- IsRetrieveMultipleAuditEnabled: 0

They should all be enabled:
- IsAuditEnabled: 1
- IsRetrieveAuditEnabled: 1
- IsRetrieveMultipleAuditEnabled: 1

[Back](../Prompt.prompt.md)