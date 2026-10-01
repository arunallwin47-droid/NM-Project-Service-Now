# Milestone 1 — High Impact Control UI Policy

## Objective

Create a ServiceNow UI Policy for the Incident table that applies additional controls when the Incident Impact is set to High.

## UI Policy Configuration

- **Name:** High Impact Control
- **Table:** Incident
- **Active:** True
- **Condition:** Impact is 1 - High
- **Reverse if false:** True
- **On load:** True
- **Application:** Global

## UI Policy Action

- **Field:** Assignment group
- **Mandatory:** True
- **Visible:** Leave alone
- **Read only:** False
- **Clear the field value:** False

## Implementation

The UI Policy is triggered when the Incident Impact is set to `1 - High`.

The UI Policy Action makes the `Assignment group` field mandatory.

When the condition becomes false, the UI Policy Action is reversed because `Reverse if false` is enabled.

## Status

**Milestone 1 — Configuration Completed**

## Evidence

ServiceNow configuration screenshots are included in this milestone folder.
