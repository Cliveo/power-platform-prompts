# Attribute review

I need help finding changes to this repo that do not align with the standards for attributes.

## Aliases

- Table = Entity
- Column = Attribute

## Context

Each entity is in a folder in src/entities.

Example: src/entities/account

Responding by going through each entity would be best.

Attributes can be found in entities, each attribute is in the attributes folder within each entitys folder.

Example: src/entities/account/attributes/*.yml

### Good description:

Descriptions:
  Description:
    '@description': Type an ID number or code for the account to quickly search and identify the account in system views.

### Missing description:

Descriptions:
  Description:
    '@description': ''

## Prompt

Please ask the user to select the table based on the entities you find. Once they have selected a table, Go through the attributes finding ones that have a missing description and input a good description. Pause after each 2 descriptions updated.

[Back](../Prompt.prompt.md)