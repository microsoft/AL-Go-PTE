# AL Extension Template - EB Development

Welcome to the AL Extension Template for EB Development. This repository contains the foundational structure and coding standards required for developing AL language extensions for Business Central.

## Table of Contents

- [Introduction](#introduction)
- [Naming Conventions](#naming-conventions)
- [File Structure](#file-structure)
- [Code Cops and Standards](#code-cops-and-standards)
- [Contributing](#contributing)

## Introduction

This template is designed to provide a standardized structure for AL extensions developed within EB Development. By following the guidelines and configurations provided here, we ensure consistency, readability, maintainability, and compliance with best practices across all projects.

## Naming Conventions

### General Rules
- **PascalCase**: All identifiers (e.g., object names, procedure names, variable names) should use PascalCase.
- **Abbreviations**: Avoid abbreviations unless they are widely recognized.
- **Prefixes**: Use appropriate prefixes for variables to clarify their scope or type.

### Object Names
- **Extensions of Existing Objects**: Object names should be based on the original object with a "PTE" suffix.
  - Example: `Sales Header PTE`
- **New Objects**: For new objects, the name should include the "PTE" suffix and clearly describe the object's purpose.
  - Example: `Customer Ledger PTE`

### Procedure Names
- Use descriptive verbs or verb phrases.
  - Example: `CalculateTotalAmount()`, `GetCustomerDetails()`

### Variable Names
- Use names that clearly convey the purpose of the variable.
  - Example: `SalesOrderHeader`, `CustomerBalance`

### Event Publisher Names
- Use `OnBefore` and `OnAfter` prefixes for event publishers.
  - Example: `OnBeforeCalculateTotals`, `OnAfterPostInvoice`

## File Structure

### Folders
- **Lowercase and Singular**: All folders should be lowercase and singular.
  - Example:
    - `/table/`
    - `/page/`
    - `/codeunit/`
    - `/report/`
    - `/enum/`

### File Names
- **Naming Pattern**: File names should follow the pattern `<ObjectNameShort>.<ObjectTypeShortPascalCase>.al`.
  - Example: `SalesHeader.Page.al`

### Root Folder
- **Source Files**: All source files should be placed in the root `src/` folder within the extension folder.

### Source Control
- **Git**: All AL files should be placed under source control using Git. The repository structure should reflect the file structure guidelines provided above.

## Code Cops and Standards

This template includes strict rules and configurations to enforce best practices in AL development. The `settings.json` and `ruleset.json` files containing the necessary Code Cop configurations can be found in this repository.

- **Code Cop Configurations**: Refer to the [`settings.json`](./.vscode/settings.json) and [`ruleset.json`](./.vscode/rulesets.json) files for the configurations used in this template.

These configurations ensure that the code adheres to EB Development’s strict standards for variable naming, object naming, code structure, and more.

## Contributing

When contributing to this repository, please follow the naming conventions, file structure, and code standards as outlined above. Adherence to these guidelines is critical for maintaining consistency across all projects.
