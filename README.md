# Salesforce access control patterns

An illustrative separation of integration runtime access and metadata development permissions using small, reviewable permission sets.

**Stack:** Salesforce DX, XML, permission design.

## What this demonstrates

Reusable implementation patterns for data integration, validation and maintainable automation. This is a curated, generalized portfolio edition. It contains no production exports, deployment history, internal access inventory or credentials. API names and source labels have been generalized where needed; configure the matching schema in your own sandbox before use.

## Getting started

For Salesforce work, use Salesforce CLI and a dedicated sandbox with the required schema and NPSP dependencies. Inspect `manifest/package.xml`, then validate with `sf project deploy start --dry-run --manifest manifest/package.xml --target-org DEMO_SANDBOX`. This repository has not been deployed or tested against a live org during portfolio preparation. 

## Source map

- `README.md`
- `force-app/main/default/permissionsets/Integration_Runtime_Access.permissionset-meta.xml`
- `force-app/main/default/permissionsets/Metadata_Developer_Access.permissionset-meta.xml`
- `manifest/package.xml`
- `sfdx-project.json`

## Validation

Python sources and JSON/XML configuration are checked locally. Apex test classes are retained where present; executing them requires a compatible sandbox. No Salesforce query, deployment, backfill or record mutation was performed during preparation. See [SECURITY.md](SECURITY.md) for data handling.
