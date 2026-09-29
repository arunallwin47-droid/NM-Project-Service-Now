# Activity 3 — Reverse Condition Test

## Objective

Verify that the High Impact UI Policy actions are reversed when the Incident Impact changes from High to Medium.

## Test Procedure

1. Open an existing Incident where Impact is set to `1 - High`.
2. Change the Impact field from `1 - High` to `2 - Medium`.
3. Verify that the High Impact UI Policy condition becomes false.
4. Verify that Assignment group is no longer mandatory.
5. Verify that the Urgency field becomes editable.
6. Complete any other required fields.
7. Click Update to save the Incident.

## Expected Result

When Impact changes from High to Medium:

- The High Impact UI Policy condition becomes false.
- Assignment group should no longer be mandatory.
- Urgency should become editable.
- The Incident should save successfully.

## Actual Result

The reverse-condition behavior was successfully verified.

After changing Impact from `1 - High` to `2 - Medium`:

- Assignment group was no longer marked mandatory.
- Assigned To was no longer marked mandatory.
- Urgency became editable.
- The High Impact validation was no longer active.
- The Incident was successfully updated after completing the required Work notes field.

## Result

**PASS — Activity 3 completed successfully.**

## Evidence

The screenshot in this folder shows the Incident after changing Impact from High to Medium and confirms the reversed UI Policy behavior.
