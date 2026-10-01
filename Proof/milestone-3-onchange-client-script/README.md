# Milestone 3 — onChange Client Script

## Objective

Create an onChange Client Script for the Incident table that automatically sets the Urgency field when the Impact is changed to High.

## Client Script Configuration

| Configuration | Value |
|---|---|
| Name | Auto set urgency for high impact |
| Table | Incident |
| UI Type | Desktop |
| Type | onChange |
| Field name | Impact |
| Active | True |
| Global | True |
| Isolate script | True |

## Script Behavior

The Client Script runs whenever the Incident Impact field changes.

When the Impact value is `1 - High`, the script automatically sets the Urgency value to `1 - High`.

It also displays an informational message confirming that the Urgency has been set to High.

The script ignores execution during form loading and when the new Impact value is empty.

## Implementation

The Client Script was created under:

**System UI → Client Scripts**

The script was configured with:

- Incident as the table
- onChange as the script type
- Impact as the triggering field
- Active enabled

The required JavaScript was added to the Script field and the record was saved successfully.

## Expected Behavior

When:

`Impact = 1 - High`

the script performs:

`Urgency = 1 - High`

and displays an informational message to the user.

## Status

**Completed — Submitted for Review**

## Evidence

The ServiceNow Client Script configuration screenshot is included in this folder.
