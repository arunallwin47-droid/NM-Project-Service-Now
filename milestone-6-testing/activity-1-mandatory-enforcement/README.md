# Activity 1 — Test Mandatory Enforcement

## Objective

Verify that a High Impact Incident cannot be saved when the **Assigned To** field is empty.

## Test Procedure

1. Navigate to **Incident → Create New**.
2. Set **Impact** to `1 - High`.
3. Leave **Assigned To** empty.
4. Click **Submit**.
5. Observe the validation result.

## Expected Result

The Incident should not be saved when:

- Impact = `1 - High`
- Assigned To = Empty

The onSubmit Client Script should display the message:

> Assigned To is mandatory for High impact incidents.

## Actual Result

The test was successfully completed.

When Impact was set to `1 - High` and Assigned To was left empty:

- Urgency was automatically set to `1 - High`.
- The Assigned To validation message was displayed.
- The Incident was prevented from being saved.

## Configuration Tested

The test validates the functionality created in the previous milestones:

- High Impact Control UI Policy
- Assignment group mandatory behavior
- Urgency automation
- onSubmit Client Script validation

## Result

**PASS — Activity 1 completed successfully.**

## Evidence

The screenshot in this folder shows the Incident form with High Impact, empty Assigned To, automatic Urgency handling, and the validation message.
